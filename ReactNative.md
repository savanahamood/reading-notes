# React Native
### getting started with react native

**1.Name three Core Components of React Native and describe what they do.**

* View (and Text)
* StyleSheet
* Component

**2.What problem does React Native solve (why call it native)?**
React Native solves the problem of duplicating development efforts for multiple mobile platforms, making mobile app development more efficient, cost-effective, and accessible to a broader range of developers who are familiar with JavaScript and React. It's called "native" because it allows you to build apps that look and feel like native apps on both iOS and Android, despite using a single codebase.


**3.What are the building blocks of a React Native app? How does that compare to a React app?**

while both React Native and React for the web share many core concepts such as components, props, state, and JSX, they differ in terms of styling, navigation, and platform-specific components. React Native is designed specifically for mobile app development, while React for the web is intended for building web applications. The key difference lies in the target platform and the associated libraries and components used to interact with it.


### expo

**1.What solution does expo provide?**
Expo provides a developer-friendly and efficient solution for building cross-platform mobile applications, offering tools, libraries, and services that simplify the development process and help you create high-quality apps for iOS and Android.

**2.Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the ____ workflow.**
Expo tries to manage as much of the complexity of building apps as possible, which is why we call it the "managed" workflow.

**3.What is the difference between React Native and Expo?**

React Native provides greater flexibility and customization options but requires more configuration, while Expo offers a simplified, managed workflow that is ideal for quick prototyping and simpler apps. Developers often choose between them based on the complexity and customization needs of their projects.


### expo snack

**Checkout this tool. What does snack allow you to do?**

* Write and Run React Native Code: Snack provides an online code editor where you can write React Native code using JavaScript or TypeScript. You can create, edit, and experiment with React Native components, views, and logic.

* Immediate Feedback: One of the main advantages of Snack is its real-time feedback feature. As you code, you can see the changes and updates to your React Native app instantly in the web browser, making it an excellent tool for rapid prototyping and testing.

* Preview on Multiple Platforms: Snack Expo allows you to preview your React Native app on multiple platforms, including iOS and Android. You can see how your app will look and behave on different devices, screen sizes, and orientations.

* Access to React Native Libraries: Snack includes a wide range of pre-installed React Native libraries and components, making it easy to incorporate functionality like navigation, animations, and UI components into your app.

* Shareable Projects: You can easily share your Snack projects with others by generating a unique URL. This is helpful for collaboration, getting feedback, or showcasing your work.

* Learning and Teaching Tool: Snack is often used as an educational tool for teaching React Native. It provides a simplified environment for learners to experiment with React Native concepts without the need for complex local development setups.

### ejecting

**1.What does “eject” mean within the context of Expo?**

Once you eject, you are responsible for managing the native development aspects of your project, which includes handling updates, configurations, and native dependencies manually.

Expo provides the "eject" command to make the transition as smooth as possible, and it generates the necessary files and configuration to help you get started with the "bare" workflow. However, it's essential to carefully consider the trade-offs and requirements of your project before deciding to eject from Expo.


**2.When should you not eject?**
you should not eject from Expo's managed workflow when it aligns with your project's goals, your team's skill level, and your app's requirements. Ejecting is a decision that should be made carefully, considering the trade-offs between simplicity and customization. Expo's managed workflow is a powerful tool for many app development scenarios, and you should leverage it unless you have compelling reasons to take on the added complexity of native development in the "bare" workflow.

**3.Why might you choose to eject?**

It's important to carefully consider your project's specific requirements and the trade-offs associated with ejecting. While ejecting offers greater flexibility and control, it also increases the complexity of your development process and requires a deeper understanding of native mobile app development. Developers should weigh the advantages of customization against the added complexity when deciding whether to eject from Expo's managed workflow.


### Resources: 

[react native](https://facebook.github.io/react-native/)

[react native basics](https://facebook.github.io/react-native/docs/tutorial)

[ejecting](https://docs.expo.io/versions/latest/expokit/eject)

[getting started with react native](https://facebook.github.io/react-native/docs/getting-started)

[expo snack](https://snack.expo.io/)

[expo](https://expo.io/)