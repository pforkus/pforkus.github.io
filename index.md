---
layout: default
title: Paul Forkus
---


<div style="text-align: center">
<img src="assets/profile1.jpg" width="200">
</div>
<h3 style="text-align: center">CS Graduate | SNHU</h3>

---

## Professional Self Assessment

---

## Artifact 1 - Software Engineering and Design

<div class="show-hide" markdown="0">
<input type="checkbox" class="read-more-state" id="artifact1" >
<div class="read-more-wrap">
<p>The artifact I chose for the software engineering and design enhancement is a mobile inventory management application I originally developed in CS-360: Mobile Architecture and Programming. Pre-enhancement, the app was a simple CRUD application that allowed users to manage inventory items using a local SQLite database that stored user credentials and inventory items. Users could create an account, login, manage their inventories, with the app even sending low inventory alerts if the user permitted.
I selected this artifact because it allowed me to consolidate multiple categories of enhancement into a single, cohesive, robust, high-quality product rather than several, smaller, unrelated artifacts. Of the work I've completed in the program, the mobile application was one of the more polished and complete artifacts and a well-suited candidate for all enhancements. Several aspects of the artifact already showcase my skills in software development. The app's adherence to the MVVM architecture demonstrates my understanding of maintainable application design and separation of concerns, while the database layer exhibits my capabilities with data modeling and persistence design. While the application was already a demonstration of my abilities, the enhancements exemplify the progress I have made since its original development.
</p>
<p class="read-more-target">The artifact was improved through the addition of several new features, tools, and QoL features for end users, as well as an entire Angular app that performs most of the same features,  and shares an API and data layer with the Android app. In the Android app, I improved the toolbar, adding a search bar to query the database for items and a navigation drawer with options to logout, exit, and to access settings. I also added an overflow menu that allows users to sort results and a toggle option to swap between a list view or a grid view. The settings option in the navigation drawer is a new activity that allows users to configure aspects of the app, like the application’s theme, font size, app permissions, and notification options. The sort button opens a bottom sheet listing the database fields and ascending/descending options, allowing users to sort items by its fields. I also implemented a filter functionality through the use of a ChipGroup that displays clickable chips with those category’s names under the toolbar. </p>
<p class="read-more-target">I did meet the two outcomes I planned to address with these enhancements: designing and evaluating computing solutions using algorithmic principles and computer science practices, and using well-founded and innovative techniques, skills, and tools for the purpose of implementing computer science solutions. The application's constant manipulation of database items necessitated utilizing algorithms and various data structures to pass data between components, aligning with outcome three. Likewise, expanding the existing Android application and building out the Angular interface demonstrates my understanding of varying architectural and design patterns, platform specific techniques, skills, and tools, aligning with outcome four.</p>
<p class="read-more-target">This enhancement deepened my understanding of Android development beyond what the original course instilled. Implementing UI components like bottom sheets and navigation drawers required learning patterns I hadn't used before, and building search, sort, and filter functionality forced me to think carefully about how data should be structured and queried to support those features efficiently. For example, I had to design solutions for populating the chip group chips with categories, and how to shape endpoints so that the mobile app could utilize the same search and sort functionality as the Angular app. I also had to think more critically about mobile-specific constraints, such as how an app should interact with device APIs, and how to handle something as seemingly simple as image storage in a way that's appropriate for the mobile context.</p>
<p class="read-more-target">The biggest challenge throughout this process was less about any single feature and more about sequencing: understanding how to add substantial new functionality while anticipating a data layer migration and implementing features in an order that avoided leaving the application in a broken or untestable state at any point. This required me to isolate changes, test incrementally, and be deliberate about the order and manner in which I introduced new features. The overall process elucidated why much of professional software development revolves around foresight and preparation, and not just on implementing functionality.</p>
</div>
<label for="artifact1" class="read-more-trigger"></label>
</div>


---

## Artifact 2 - Data Structures and Algorithms
<div class="show-hide" markdown="0">
<input type="checkbox" class="read-more-state" id="artifact2">
<div class="read-more-wrap">
<p> The data structure and algorithms enhancements were performed on the same mobile inventory tracking application used for the previous enhancement. The app was originally a simple CRUD application that allowed users to manage their inventories, leveraging a local SQLite database to persist user credentials and inventory items. Users could create an account, login, and then manage their inventories, receiving SMS alerts when items needed replenishment. 
</p>
<p>I chose to perform all enhancements on the mobile inventory application as this allowed me to concentrate my efforts on delivering a singular, highly-polished application where the enhancements build off and reinforce each other, rather than enhancing three artifacts that existed in isolation. As a result, reviewers can focus on one codebase, allowing them to spend their limited time evaluating my engineering rather than switching between projects. </p>
<p>While the application already leveraged numerous data structures and algorithms to communicate, store, and retrieve data, such as hash maps, lists, and arrays, their use was insufficient to demonstrate my skills leveraging data structure and designing algorithms. To address this, I began looking for aspects of the application that could be improved meaningfully through the use of data structures and algorithms. </p>
<span class="read-more-target">
  <p>The solution came with the creation of the search feature, and the inspiration to implement a search suggestion feature. The feature consists of a  prefix trie populated with all item names that would observe any text typed in the search view via onTextQueryChanged and use that input to traverse the tree and retrieve matching names. I chose to implement this feature as it not only satisfies the requirements, it introduces data structures and algorithms to provide functionality that is relevant to the app’s goal, as it provides real value by making searches faster and more accessible to those who are less dexterous. The trie’s implementation and integration into the Android app demonstrates my ability to research, design, and deploy data structures that are appropriate, and algorithms that are thoughtfully designed. </p>
<p>I met all the course outcomes I planned to meet with this requirement. However,  I made more progress with outcome five this week than I intended. Beginning the data structure and algorithm enhancement necessitated that I first complete the database enhancement as the search suggestion feature relied on the search functionality and the new database. Due to this, I migrated both database collections and also implemented user credential hashing and salting. As I was now sending raw credentials over HTTP for server-side hashing, I recognized that HTTP was now insufficient to protect those credentials in transit and resultingly deployed the backend code to Render, so that connections would be automatically secured with HTTPS. While I may have been able to create my own certificates for SLS/TLS, I was uncertain how or whether Android would accept self-signed certificates. As a result, the implementation of these two tangential features helped me accomplish partial completion of outcome 5 while working on the trie. </p>
<p>My trie implementation aligns with both outcome three and four. It demonstrates outcome three by showcasing my ability to evaluate computing solutions using algorithmic principles and computer science practices, while its integration into the Android application demonstrates alignment with outcome four, as it demonstrates my proficiencies with mobile development and adherence to the MVVM architecture.</p>
<p>This aspect of the capstone was likely the least involved, yet the prerequisite infrastructure was rather involved. As such, completing this week’s enhancement required me to plan ahead and adhere to a strict deadline. Additionally, I learned how to implement a prefix trie, and how to perform various operations on the nodes in that trie. One challenge I faced with the trie involved deletion; specifically, if multiple entries exist with the same name, one item’s deletion should not remove the name from the trie, as the trie only adds unique names. This resulted in adding a name occurrence tracker that would be referenced on item deletion to ensure items were not removed unless it was the last matching entry. The biggest challenges this week were actually related to establishing the sort and search functionality in preparation for the search suggestion feature. Overall, I enjoyed learning how to implement a prefix trie and figuring out how integrate it into a meaningful feature for my application.</p>
</span>
<label for="artifact2" class="read-more-trigger"></label>
</div>

---

## Artifact 3 - Databases

---

## Original Artifact

- [Android Inventory Tracking App](https://github.com/pforkus/inventory-tracking-original)

---

## Finalized Artifact

- [Angular Interface / Express API](https://github.com/pforkus/CS499-1) <br>
- [Android Application](https://github.com/pforkus/CS499)

---

- [Before & After Comparison](comparison.html)

---

## Code Review
Prior to implementing any enhancements on the mobile inventory tracking application, I thoroughly reviewed the code to identify vulnerabilities, logical issues, and bad design practices to ensure that enhancements are built on a solid foundation. If you are interested in my observations and thought process throughout, you can watch along [here](https://www.youtube.com/watch?v=7f9-uHa4kbs).

---

