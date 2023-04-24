# Lab Report 2 - Servers and Bugs
## Part 1 - Write a web server called StringServer
`import java.io.IOException;`
`import java.net.URI;`

`class Handler implements URLHandler {

   String s;
    public String handleRequest(URI url) {`
        `if (url.getPath().contains("/add-message")) {
            String[] parameters = url.getQuery().split("=");
            String kp;
            if (s != null) {
                kp = s + "\n" + parameters[1];
                return kp;
            }
            s = parameters[1];
            return s;
        }
        return "404 Not Found!";
    }
}`
    `class StringServer {
        public static void main(String[] args) throws IOException {
            if(args.length == 0){
                System.out.println("Missing port number! Try any number between 1024 to 49151");
                return;
            }
    
            int port = Integer.parseInt(args[0]);
    
            Server.start(port, new Handler());
        }
    }`
