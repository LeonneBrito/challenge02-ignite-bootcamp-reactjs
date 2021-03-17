<img alt="Ignite" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F2fbacb7a-e460-44a3-8fc5-e66f96dae148%2Fcover-reactjs.png?table=block&id=51e4099a-6e2f-4d4b-ae94-f9fe75bb769d&width=5120&userId=1b109781-8635-4162-80d6-714377721793&cache=v2" />

<h3 align="center">
Challenge 02: Componentizing the application
</h3>

<p align="center">	
   <a href="https://www.linkedin.com/in/leonne-sousa-brito/">
      <img alt="LeonneBrito" src="https://img.shields.io/badge/-LeonneBrito-5965e0?style=flat&logo=Linkedin&logoColor=white" />
   </a>
  <img alt="Languages" src="https://img.shields.io/github/languages/count/LeonneBrito/challenge02-ignite-bootcamp-reactjs?color=%235963C5" />
  <img alt="repo-size" src="https://img.shields.io/github/repo-size/LeonneBrito/challenge02-ignite-bootcamp-reactjs?color=%235761C3" />
  <img alt="lastcommit" src="https://img.shields.io/github/last-commit/LeonneBrito/challenge02-ignite-bootcamp-reactjs?color=%235761C3" />
  <img alt="License" src="https://img.shields.io/github/license/LeonneBrito/challenge02-ignite-bootcamp-reactjs?color=%235E69D7" />
  <img alt="Issues" src="https://img.shields.io/github/issues/LeonneBrito/challenge02-ignite-bootcamp-reactjs?color=%235965E0">
  <a href="mailto:contato@leonnebrito.com.br">
   <img alt="Email" src="https://img.shields.io/badge/-contato%40leonnebrito.com.br-%23525DCB" />
  </a>
</p>

## :rocket: About the challenge

In this challenge, you will have to create an application to train what you have learned so far in ReactJS

This will be an application where your main objective is to refactor a page for listing films according to genre.

The application is already fully functional but a large part of its code is directly in the `App.tsx` file. To solve this in the best way, it is necessary to divide the application into ** at least ** two main parts: sidebar and the main content that has the header and the list of films.

- The application has only one main feature, which is the listing of films;
- In the sidebar it is possible to select which category of films should be listed;
- The first category on the list (which is "Action") should start as marked;
- The application header has only the name of the selected category that must change dynamically.

## :construction_worker: Preparing for the challenge

For this challenge, in addition to the concepts seen in class, we will use some new things to make our application even better. So, before going directly to the challenge code, we will explain a little bit about Fake API with JSON Server.

## Fake API with JSON Server

Just as we use MirageJS in module 2 to simulate an API with transaction data from the dt.money application, we will use JSON Server to simulate an API that has the information of genres and films.

Navigate to the created folder, open it in Visual Studio Code and execute the following commands in the terminal:

```bash
yarn
yarn server
```

Then you will see the message:

<img alt="server" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F1abc3356-2936-4106-a4fe-a3fc8efd1373%2FUntitled.png?table=block&id=7fe88f6f-62c6-45c7-a898-d1672dbbe6bd&width=1420&userId=&cache=v2" />

Note that he started a fake API with the `/genres` and` /movies` resources in `localhost` on port` 3333` from the information in the [server.json] file (https://github.com/rocketseat-education/ignite-template-componentizando-a-aplicacao/blob/main/server.json) located at the root of your project. Accessing these routes in your browser, you can see the return of the information already in JSON:

<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F12a3c689-264b-4bd4-8515-730dfe8dd407%2FUntitled.png?table=block&id=e27d872a-13a6-4c37-ba61-34b7fb2f74dd&width=850&userId=&cache=v2" />
<img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F400b84d4-2de4-4cd3-aef2-139f3103e9f6%2FUntitled.png?table=block&id=c2e1b5cd-c028-45b6-9319-b88aab9b0ece&width=670&userId=&cache=v2" />

That way, you just need to consume these API routes normally with Axios.

## :wrench: What should I edit in the application?

With the template already cloned, the dependencies installed and the fake API running, you must create **at least** the SideBar and Content components that already have the files created.
The files to be edited are:

- **src/App.tsx**
This component contains the entire application with the exception of the `Button` component that does not need to be changed and `Icon` that also does not need to be changed.
- **src/components/Content.tsx**
This component, still empty, must have all the logic and body responsible for the header and content of the application (section outlined in red):

<img alt="screen1" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fff7c8a12-50d1-4a20-a680-9085d0bd6823%2Fexample.png?table=block&id=641fa56e-763e-48f3-8a2b-1bf93007de1b&width=1250&userId=&cache=v2"/>

- **src/components/SideBar.tsx**
This component, also empty, must have all the logic and body responsible for the section that contains the title of the site and the navigation part to the left of the page (section outlined in red):

<img alt="screen2" src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F88f057c2-d29a-4b0d-b9ed-f11385e09030%2Fexample.png?table=block&id=673530e2-c5dc-4813-97f2-37c4dfabc170&width=1340&userId=&cache=v2" />

If you prefer, you can also componentize some other parts of the application, such as the header, but that is not a requirement of this challenge 🚀

# :page_facing_up: License

This project is under a license [MIT](./LICENSE).

Challenge proposed with 💜 by Rocketseat 👋 [Join this great community!](https://discordapp.com/invite/gCRAFhc)
