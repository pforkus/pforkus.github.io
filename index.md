<style>
summary {
  cursor: pointer;
  color: #0366d6;
  list-style: none;
  display: inline;
}
summary::-webkit-details-marker {
  display: none;
}
summary:hover {
  text-decoration: underline;
}
</style>

---

layout: default
title: Paul Forkus

---

<div style="text-align: center">
<img src="assets/profile1.jpg" width="200">

</div>
<h3 style="text-align: center">CS Graduate | SNHU</h3>

---

## About Me

---

## Artifact 1

<p>The artifact is a mobile inventory management application originally built for CS-360: Mobile Architecture and Programming. It allows users to log in, view, add, edit, and delete inventory items, with data originally persisted locally using Android's Room database.
I selected this artifact because it allowed me to consolidate multiple categories of enhancement into a single, cohesive, robust, high-quality product rather than several, smaller, unrelated artifacts. Of the work I've completed in the program, the mobile application was one of the more polished and complete artifacts and a well-suited candidate for all enhancements. Several components of the preexisting artifact already showcase my skills in software development. The app's adherence to the MVVM architecture demonstrates an understanding of maintainable application design and separation of concerns. The database layer, including the DAO and entity definitions, demonstrates my proficiency with data modeling and persistence design.</p>

<details>
<summary>Read More</summary>
<p>The artifact was improved through the addition of several new features, tools, and improvements. I added several elements to the toolbar, including a search bar to query the database for items. I implemented a hamburger menu that opens a drawer with options to logout, exit, and to access settings. The settings activity is a new activity that allows users to change the application's theme or font size, in addition to providing permission and notification options. I added a sort button that opens a bottom listing the database fields and ascending/descending options. I addressed existing formatting issues and expanded the item dialog fragment to contain the fields required for the new item schema. I also implemented filter functionality through the use of a ChipGroup that displays chips with the current inventory's categories. Finally, I added an option in the overflow menu to toggle between the application's list and grid layouts for displaying inventory items. In addition to my work on the Android application, I simultaneously built an Angular app that interfaces with the same database and contains most of the same features.</p>
<p>I did meet the two outcomes I planned to address with these enhancements: designing and evaluating computing solutions using algorithmic principles and computer science practices, and using well-founded and innovative techniques, skills, and tools for the purpose of implementing computer science solutions. The application's constant manipulation of database items necessitated utilizing algorithms and various data structures to pass data between components, aligning with outcome three. Likewise, expanding the existing Android application and building out the Angular interface demonstrates my understanding of varying architectural and design patterns, platform specific techniques, skills, and tools, aligning with outcome four.</p>
<p>This enhancement deepened my understanding of Android development beyond what the original course instilled. Implementing UI components like bottom sheets and navigation drawers required learning patterns I hadn't used before, and building search, sort, and filter functionality forced me to think carefully about how data should be structured and queried to support those features efficiently. For example, I had to design solutions for populating the chip group chips with categories, and how to shape endpoints so that the mobile app could utilize the same search and sort functionality as the Angular app. I also had to think more critically about mobile-specific constraints, such as how an app should interact with device APIs, and how to handle something as seemingly simple as image storage in a way that's appropriate for the mobile context.</p>
<p>The biggest challenge throughout this process was less about any single feature and more about sequencing: understanding how to add substantial new functionality while anticipating a data layer migration and implementing features in an order that avoided leaving the application in a broken or untestable state at any point. This required me to isolate changes, test incrementally, and be deliberate about the order and manner in which I introduced new features. The overall process elucidated why much of professional software development revolves around foresight and preparation, and not just on implementing functionality.</p>
</details>


---

## Artifact 2

---

## Artifact 3

---

## Original Artifact

- [Android Inventory Tracking App](https://github.com/pforkus/inventory-tracking-original)

---

## Finalized Artifact

- [Angular Interface / Express API](https://github.com/pforkus/CS499-1) <br>
- [Android Application](https://github.com/pforkus/CS499)


---

## Code Review
Prior to implementing any enhancements on the mobile inventory tracking application, I thoroughly reviewed the code to identify vulnerabilities, logical issues, and bad design practices to ensure that enhancements are built on a solid foundation. If you are interested in my observations and thought process throughout, you can watch along [here](https://www.youtube.com/watch?v=7f9-uHa4kbs).

---

