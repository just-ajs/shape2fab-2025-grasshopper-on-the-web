<img src="https://github.com/user-attachments/assets/3ea261ab-dcca-421b-ad97-c7b0693d3ebe" width=100>


# Grasshopper on the Web: Creating Websites with Rhino.Compute, Vue, and Three.js. 

Shape to Fabrication 2025 workshops led by David Andres Leon, Justyna Szychowska and Andy Payne.

Learn to build a custom web interface for real-time control and display of Grasshopper definitions. In this workshop, you will learn how to prepare your Grasshopper scripts to run on the web with Rhino.Compute. You will also explore the basics of Vue.js, a user-friendly web framework, enabling you to create a beautiful and reusable web interfaces that can control your Grasshopper definition inputs. Additionally, you will gain experience with Three.js web geometry library to develop dynamic and custom 3D scenes in your website. 

## Prerequisites
[Installation Instructions](https://docs.google.com/document/d/1xL8lZSxwkRQMDbWF1rpV9iVWnkFTFZEInC_brpCEzoA/edit?usp=sharing)

- Rhino 7
- Hops
- Visual Studio Code
- Node
- Git
- Github


## Run project locally

### Start Rhino.Compute

Start your local Rhino.Compute server either by running your Grasshopper (with Hops installed).

You know that Rhino.Compute is running if you can see in your console `Now listening on..`

![image](https://github.com/user-attachments/assets/127ae448-e58b-4bb8-b456-23969d49c064)


When you have Rhino.Compute running, have a look at the number of the localhost. The example above has a localhost number `6500`. This number needs to match the host number in the `source/scripts/compute.js` file (line 6).

`RhinoCompute.url = "http://localhost:6500/"`

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

#### Common Issues

##### npm execution policy
If you are seeing errors when trying to run npm commands, run this command in Powershell to enable running scripts.

`Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted`

##### .NET framework
If you get error in the console when running Rhino.Compute that says that there is .net missing, make sure you have .net8 installed on your machine. You can check that by running command `dotnet --list-runtimes` in your console. 

### References
* https://developer.rhino3d.com/guides/compute/
* https://threejs.org/
