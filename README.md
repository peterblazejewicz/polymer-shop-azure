# Polymer Shop demo application on Azure

A Polymer shop demo client app with Dotnet Kestrel server and Azure deployment script

## Generate Polymer app with `polymer-cli`

```
  /\˜˜/   /\˜˜/\   
  /__\/   /__\/__\    Polymer-CLI
 /\  /   /\  /\  /\ 
/__\/   /__\/  \/__\  The multi-tool for Polymer projects
\  /\  /\  /   /\  /
 \/__\/__\/   /__\/   Usage: `polymer <command> [options ...]`
  \  /\  /   /\  /  
   \/__\/   /__\/   


Available Commands

  build   Builds an application-style project                     
  help    Shows this help message, or help for a specific command 
  init    Initializes a Polymer project                           
  lint    Lints the project                                       
  serve   Runs the polyserve development server                   
  test    Runs web-component-tester
  ```

You can use `polymer-cli` tool to scaffold your client side application: [https://github.com/polymer/polymer-cli](https://github.com/polymer/polymer-cli)

## Scaffold Dotnet web application over Polymer content

You can use tool like `generator-aspnet` or `dotnet-cli new` commands to generate ASP.NET content over your client side code and use Git to review changes. This project was scaffolded with `Empty Web Application` project type and later updated to use static web site feature and custom hosting configuration for Kestrel server

## Author

@peterblazejewicz