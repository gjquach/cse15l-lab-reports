# Lab Report 3
## Part 1: Search Engine
```
import java.io.IOException;
import java.net.URI;
import java.util.ArrayList;

class Handler implements URLHandler {
    ArrayList<String> listOfWords = new ArrayList<>();
    public String handleRequest(URI url) {
        if (url.getPath().contains("/add")){
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")) {
                listOfWords.add(parameters[1]);
            }
            return String.format("Added:" + parameters[1]);
        }else if (url.getPath().contains("/search")){
            ArrayList<String> wordsWithSub = new ArrayList<>();
            String[] parameters = url.getQuery().split("=");
            if (parameters[0].equals("s")) {
                for(int i = 0; i < listOfWords.size(); i++){
                    if(listOfWords.get(i).contains(parameters[1])){
                        wordsWithSub.add(listOfWords.get(i));
                    }
                }
                return String.format("List of words with substring:" + wordsWithSub);
            }
        }else{
            return "Add a String!";
        }
        return "Add a String!";
    }
}

class SearchEngine {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }
        int port = Integer.parseInt(args[0]);
        Server.start(port, new Handler());
    }
}
```
![add books to list](addBooks.png)
- Calls the handleRequest method
- url = localhost:4000/add?s=books
- parameters = [s, books]
- listOfWords = [books]

![add cookbook to the list](addCookbook.png)
- Calls the handleRequest method
- url = localhost:4000/add?s=cookbook
- parameters = [s, cookbook]
- listOfWords =[books, cookbook]

![addWatch](addWatch.png)
- Calls the handleRequest method
- url = localhost:400/add?s=watch
- parameters = [s, watch]
- listOfWords = [books, cookbook, watch]

![test](list.png)
- Calls the handleRequest method
- url = localhost:4000/search?s=book
- parameters = [s, book]
- wordsWithSub = [books, cookbook]

## Part 2