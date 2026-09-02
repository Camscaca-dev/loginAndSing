# loginAndSing
Cadastro e Login

###index.ts

const srv = bun.server ({

     port:3000,
     
     routes: {
          "/teste":{
          GET: async (req) => {
          const url = new URL(req.url)
          const search = url.searchParams
          const nome = search.get("nome")
          console.log(nome)
          new Response("Cams_GET"),
          },
          
          POST: async (req) => { 
          const body = await req.body.text()
          console.log(body)
          return new Response("Cams_POST"),
          
     },
     DELETE () =>  new Response("Cams_DELETE"),
     PUT () => new Response("Cams_PUT")
}
})

  Console.log(`Rodando no pc ${srv.url}`)


usando o bruno portable fizemos testes das portas

"http://localhost:3000/teste?nome=daniel"

protocolo: http "://"
host: endereço
porta: acesso pra uma pagina ou parte especifica do servidor, identidade do serviço
servidor: é um software

url: universal, resource, locator

rodar com --watch sempre pra ir atualzando, c nao tem q para e rodar dnv a cada atualização

tamo tentando testra as rotas
