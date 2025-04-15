
# Grasshopper on the Web: Creating Websites with Rhino.Compute, Vue, and Three.js. 

Learn to build a custom web interface for real-time control and display of Grasshopper definitions. In this workshop, you will learn how to prepare your Grasshopper scripts to run on the web with Rhino.Compute. You will also explore the basics of Vue.js, a user-friendly web framework, enabling you to create a beautiful and reusable web interfaces that can control your Grasshopper definition inputs. Additionally, you will gain experience with Three.js web geometry library to develop dynamic and custom 3D scenes in your website. 



## Prerequisites
[Installation Instructions](https://docs.google.com/document/d/17hXwG_7kRkxQQLEcFkq0k_4eD659sB39gbIIzKDqi_0)
- Rhino 7
- Hops
- Visual Studio Code
- Node
- Git
- Github


## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).

 
## Run project locally


### Start Rhino.Compute

Start your local Rhino.Compute server either by running your Grasshopper (with Hops installed).

You know that Rhino.Compute is running if you can see in your console `Listening on..`

![image](https://github.com/just-ajs/aectech-2024-kpf-ttcore-worskhop/assets/35227625/f41a0b9b-d4a8-4e07-9fdf-4051a14b02a8)

When you have Rhino.Compute running, have a look at the number of the localhost. The example above has a localhost number 8081. This number needs to match the host number in the `source/scripts/compute.js` file (line 6).


![image](https://github.com/just-ajs/aectech-2024-kpf-ttcore-worskhop/assets/35227625/85246a48-a91d-41e6-aaca-4654cabc79e4)

If your Rhino.Compute localhost number is different, adjust `compute.js` file to match it. 


### Run front-end

In the terminal, run following commands:

#### Install packages needed to run the project

```sh
npm install
```

#### Compile and Hot-Reload for Development

```sh
npm run dev
```

#### Compile and Minify for Production

```sh
npm run build
```

#### Issues:

##### npm execution policy:
`Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted`

#### .NET framework
* Update .NET to 8.0
* Make sure you are using that .NET version in `%AppData%/McNeel/Rhinoceros/packages/8.0/Hops/0.16.18/compute.geometry/compute.geometry.runtimeconfig.json`

### References
* https://developer.rhino3d.com/guides/compute/
* https://threejs.org/
