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

protocolo: http "://"
host: endereço
porta: acesso pra uma pagina ou parte especifica do servidor, identidade do serviço
servidor: é um software

url: universal, resource, locator

rodar com --watch sempre pra ir atualzando, c nao tem q para e rodar dnv a cada atualização

tamo tentando testra as rotas
