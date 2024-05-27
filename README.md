package main

 


func createSnippet(w. ResponseWriter, r*http.Request) {

    

    if r.Method != http.MethodPost {

        
        

        w.WriteHeader(405)

        w.Write([]byte("GET-Метод запрещен!"))

        return

    }

 

    w.Write([]byte("Создание новой заметки..."))

}
