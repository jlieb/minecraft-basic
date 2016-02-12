# minecraft-basic

This is a cookbook that installs the vanilla [Minecraft](http://minecraft.net) server.

I have written a post on how to use this cookbook and deploy it to Digital Ocean [here](http://jjasghar.github.io/blog/2015/08/23/lets-build-a-minecraft-server-with-chef/).

I took a lot of this setup from [minecraft.gamepedia.com](http://minecraft.gamepedia.com/Setting_up_a_server). There might be some things you'd like to tweak, so please take a look at the configuration options. If you would like to configure your Minecraft server, you need to either use override attributes, or edit the [attributes/default.rb](attrubutes/default.rb) and upload your cookbook to a Chef Server. A brief explanation for the different options are located in the [attributes/default.rb](attrubutes/default.rb).

## Setting Operator
Configure the server by editing the server.properties file, the format for which is explained here. Be certain to edit the file with a text editor that does not add formatting (e.g., for italics). Additional configuration may not be necessary as many servers run fine from the default values.
Add your username to the admin.txt and/or ops.txt (newer Minecraft versions may not have an admin.txt file). Ops.txt and admin.txt determine who may execute server commands. In other words, operator ("op") privileges allow you to control certain aspects of the game (e.g., teleporting players). Op privileges may also be granted from the server GUI: type "op " and it will automatically add to the ops.txt file.

## Contributing
1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write your change
4. Write tests for your change (if applicable)
5. Run the tests, ensuring they all pass
6. Submit a Pull Request using Github

## License and Authors
- Author:: JJ Asghar (jj@chef.io)

```text
Copyright 2015 JJ Asghar

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
