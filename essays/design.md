---
layout: essay
type: essay
title: "Structured Solutions"
published: true
date: 2025-12-05
labels:
  - Software Engineering
  - Design Patterns
  - Web Development
  - Design
---

## The Architecture Behind the Scenes

If you think about software like a campus building, the code is not just a pile of bricks—it’s beams, hallways, fire escapes, and doors arranged with intention. Architects rely on proven structural blueprints, and software developers rely on something similar: design patterns. These patterns are not copy-and-paste chunks of code; they are repeatable solutions for recurring problems, born from decades of engineers discovering what works—and what collapses under stress. When we began designing the UH Mānoa Lost & Found web application, we quickly realized that without these architectural patterns, the system would become a maze of tangled logic and unpredictable behavior. Instead, by borrowing the “blueprints” of those who solved similar problems before us, we could construct a system that was organized, scalable, and surprisingly elegant.

## Patterns as Storytellers

One of the delightful moments in building our lost-and-found platform was recognizing how naturally certain design patterns fit our workflow—almost as if they were characters in a story. Consider the Observer Pattern: it appears whenever users want to be notified about a relevant change. In our case, students subscribe to alerts for items matching specific keywords or locations, and the system sends notifications whenever a new found item is posted. The Observer pattern becomes the messenger in our story, ensuring that owners hear about potential matches instantly. Meanwhile, the Factory Pattern quietly works behind the scenes each time a new Lost or Found post is created—assembling objects with consistent structure regardless of category, building, or data source. Even the Strategy Pattern makes an appearance: our filtering system (category, building, date, keywords) swaps among multiple filtering strategies without requiring new logic each time. These patterns shape the story without calling attention to themselves, allowing the system to behave cleanly and predictably.

## How the Patterns Shape Our Final Application

By the time our project’s architecture took form, the design patterns we chose felt less like academic concepts and more like essential tools that made everything fit together. The MVC pattern became our overarching narrative frame: mockups, routes, components, and (eventually) backend endpoints cleanly separated visual layout from underlying behavior. The Singleton Pattern appears in shared services, such as our Locations Directory data source or future authentication handler—ensuring a single authoritative source for campus offices and user credentials. Even the Decorator Pattern subtly influenced our approach to item metadata: photos, timestamps, verification status, and recovery instructions “decorate” a base item object without altering its core identity. By embracing these patterns, our project didn’t just meet requirements—it gained a structure that will withstand new features, new team members, and new Manoa students for years to come. In the end, design patterns became less of a textbook topic and more like the architectural language that allowed our team to build something coherent, functional, and genuinely useful to the UH community.
