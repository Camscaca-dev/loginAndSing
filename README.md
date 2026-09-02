# loginAndSing
Cadastro e Login

###index.ts

const srv = bun.server ({
     port:3000,
     routes: {
          "/teste":{
          GET () => new Response("Cams_GET"),
          PUT () => new Response("Cams_PUT"),
          DELETE () =>  new Response("Cams_DELETE"),
          POST () =>  new Response("Cams_POST"),
         
     }
}
})

  Console.log(`Rodando no pc ${srv.url}`)


usando o bruno portable fizemos testes das portas
