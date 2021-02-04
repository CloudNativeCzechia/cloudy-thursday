# Cloudy Thursday ep. 5 - Cloud native predictions
#cncz #show #notes

Every year seems to be wild on new technologies, this year is no different and there are some interesting predictions that might happen, as Chris noted in his report https://www.aniszczyk.org/2021/01/19/cloud-native-predictions-for-2021-and-beyond/.

## Raise of cloud IDEs

Comercial companies like: https://www.gitpod.io/ are making the development easier for everyone on any harware. This is not really supripsing honestly.

Red Hat's https://developers.redhat.com/products/codeready-workspaces/overview is an integration of the OpenShift and RH tooling to provide all-in-one intgrated solution for fast onboarding and smooth development.

Google has one calls it "Cloud shell" https://cloud.google.com/blog/products/application-development/introducing-cloud-shell-editor and it integrates all tools needed to build application for Google cloud.

AWS also has one named "cloud9" https://aws.amazon.com/cloud9/ which also includes all tools needed to build for AWS.

Unsuprisingly Github Codespaces (integrates well with Azure, although the support is still in progress) https://visualstudio.microsoft.com/cs/services/github-codespaces/ offers tools to build in the cloud (or on desktop) for Azure.

There is also the original tool Eclipse Che https://www.eclipse.org/che/ that offers you the ability to build your cloud IDE for on-premise solution https://www.eclipse.org/che/. Also it seems that most cloud editors are using Che as a base.

Moreover the clouds are offering you a way to operate them using nothing but browser utilizing cloud shell. Azure https://docs.microsoft.com/en-us/azure/cloud-shell/overview and AWS https://aws.amazon.com/cloudshell/. This enables quick and simple operations without prior local setup.

The whole development seems to now be situated directly onto the "world computer" in the cloud, which seems to be the direction as more and more developers are onboarded and requiements for faster onboarding are here.


## K8s on the edge

Great comment aim at k8s evolution and its move towards the edge. What I am missing is the definition what the edge is.

One of the topics that is told again and again is the use of K8s for telco as the means to run original VNFs https://en.wikipedia.org/wiki/Network_function_virtualization, this means that the K8s would run in the radio tower near you and it could be really small cluster. Seems like an overkill? Actually no, the towers already contains servers running network funsctions and doing who know what with data flowing thourgh.

Other usecase would be a large shopping mall using the K8s as orchestrator for its registers. In this case the registers would be working as a nodes and masters would manage the workloads. 

Finally one possible (still in research) usecase is IOT farm where all the iot devices are nodes for the one large cluster. This would require change of operation as workloads are targeted directly for the end node, but it is definitely doable.

## Wasm and its use in the cloud

Web assembly seems to be the next big thing, and I do understand the excitment. The possibility to run code written in different languages within the sandbox is powerful.

Moreover thanks to krustlet https://krustlet.dev/ kubernetes is able to run webassembly workloads supporting WASI https://wasi.dev/ as a kubernetes node. This is similar to what kubevirt does https://kubevirt.io/ thanks to kubernetes extensibility.

I am actually expecting similar thing to be dne for graalvm https://www.graalvm.org/ as it matures and offers similar possibilities.

## Rise of finops

On the show we hosted few guests that had the experince building cloud workload to support financial instituions and it is not really suprising, that many banks and even states are now progressing into the financial computations in the cloud.

On top of that withing the latest cryptocurrency boom, I believe it is here with us for the near future. We will be witnesses to see how large banks and states figure out a mechanism to incorporate its cryptocurrency as part of state currency.

As for now, may banks are now deploying to the cloud to save money and enable them to operate faster.

The operaties were inevitable, but now they have shiny new buzzoword.

## More rust

Well, this is again not suprising. Rust now has the similar path as golang had. It is hyped with great promises of safety, also it is shiny and new. This is enough for developers to use it and force it in their organization. More it is used the more chance for it to stay.

With support from microsoft, google, amazon and original firefox, Rust has strong foundations for developers to believe it is the new big thing and they should invest their time in it.

This was already visible a year back, as the conference poped up and young developers started rumbling about rust and small pet projects strated to appear as a means of exploration.

And yes it offers great features for low level tools in the cloud.

## GitOps

I believe we talkend about this last time. Managing infra as a code is a good practice and more and more organization starts to understand that having the infra in the code is the best way of documenting what is running where.

## Service catalogs

Which is a shiny way of defining developer portal much like openshift UI. All-in-one place for monitoring, logging and creating new stuff. 

Let us be honest, our lives are getting more complex due to the fact that we are building larger and more complicated systems. Service catalogs should be the way for us to get overview of the system and give us the ability to interact with it.

However at this stage, I am not very convinced we will get there soon. 

## Cross cloud

If there is anything I remember from last year big tech events, it is the word "hybrid cloud" and "multicloud strategy". Now, if you are small company this is not for you. However if you are big airline with hundreds of plain in the air and thousands of people waiting on the ground. You need insurance your system is 100% up and running.

Companies are starting to take this seriously also this year, as every big cloud provider tries hard to introduce lockin.
Again honestly, true cross cloud is hard and it is not write once run everywhere. But with right tooling we are getting there.

Great example is openshift which offers the same stable platform on-premise or in the AWS or Azure. This means you can move your workload more od less between clouds.

## eBPF

Strong tool that enables the other tooling to help with cloud native tools. But none of us is an expert on this topic.

