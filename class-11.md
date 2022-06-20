# Class 11 - Topics. Audio, Video, Images

## Video and Audio Content

We use audio and video in HTML by using two tags/elements:

    <video> 
        <source>

    <audio>

        Attributes to both: src , controls .. 
    Example
    <video src="rabbit320.webm" controls>
      <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.webm">link to the video</a> instead.</p>
    </video>

- The Video tag embeds a video. The src attribute creates a path to the video. The controles is used to start and stop media, or adjust volume. A paragraph inside the < video > tags is called **fallback content*,* if it doesn't work.

- Audio files use formats including MP3, MP4, and WebM, which are container formats. Audio players will often play an audio track directly, like an MP3 or Ogg file, which don't need containers.

- Within the < video > tags, there is a < source > tag. This acts the same as src attribute. < source > has a **type** attribute, which contains the MIME type of the file specified by the < source >. Browsers can use type to skip videos they don't understand. IF type isn't included, browsers will load and try to play each file until they get one that works.

Example of < video > features:

    <video controls width="400" height="400"
        autoplay loop muted preload="auto"
        poster="poster.png">
    <source src="rabbit320.mp4" type="video/mp4">
    <source src="rabbit320.webm" type="video/webm">
    <p>Your browser doesn't support HTML video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
    </video>  

New attribute features for this (which can be used in CSS) include:

- width and height
- autoplay
- loop
- muted
- poster
preload

< Audio > works similarly to < video >

Example:

    <audio controls>
    <source src="viper.mp3" type="audio/mp3">
    <source src="viper.ogg" type="audio/ogg">
    <p>Your browser doesn't support HTML5 audio. Here is a <a href="viper.mp3">link to the audio</a> instead.</p>
    </audio>

Audio element does not support height/width attributers. It does support the < track > tag and WebVTT, which is a format for writing text files with multiple strings of text .

---

## CSS Grid Guide

CSS Grid Layout is a 2-D, grid based laout system that solves past laout problems.

To use CSS Grid, we define a container element as a grid using:

        display:grid

    Set the column and row sizes using

        grid-template-columns
        grid-template-rows

    Child element into grid are

        grid-column
        grid-row

---

### Grid Container Example:

    <div class="container">
        <div class="item item-1"> </div>
        <div class="item item-2"> </div>
        <div class="item item-3"> </div>
    </div>

---

### Grit Item Example:

    <div class="container">
        <div class="item"> </div>
        <div class="item">
            <p class="sub-item"> </p>
        </div>
        <div class="item"> </div>
    </div>

---

### Grid Line

The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. 

![Grid Line](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-line.svg)

---

### Grid Cell

The space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid. 

![Grid Cell](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-cell.svg)

---

### Grid Track

The space between two adjacent grid lines. You can think of them as the columns or rows of the grid.

![Grid Track](https://css-tricks.com/wp-content/uploads/2021/08/terms-grid-track.svg)

---

### Grid Area

The total space surrounded by four grid lines. A grid area may be composed of any number of grid cells. 

![Grid Area](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-area.svg)

---

Properties for Parent (grid container):

Within the display, we can use "grid" or "inline-grid."

    .container {
        display: grid | inline-grid;
    }

Properties for Children (grid items):

These items include:

    grid-column-start
    grid-column-end
    grid-row-start
    grid-row-end

Values include:

< line >
span < number >
span < name >
auto

    .item {
    grid-column-start: <number> | <name> | span <number> | span <name> | auto;
    grid-column-end: <number> | <name> | span <number> | span <name> | auto;
    grid-row-start: <number> | <name> | span <number> | span <name> | auto;
    grid-row-end: <number> | <name> | span <number> | span <name> | auto;
    }

Example:

    .item-a {
    grid-column-start: 2;
    grid-column-end: five;
    grid-row-start: row1-start;
    grid-row-end: 3;
    }



[ https://css-tricks.com/snippets/css/complete-guide-grid/ ]

## Responsive Images

We can use two attributes to provide source images to help browser pick the right one:

    srcset
    sizes

    Example:

    <img srcset="elva-fairy-480w.jpg 480w,
                elva-fairy-800w.jpg 800w"
        sizes="(max-width: 600px) 480px,
                800px"
        src="elva-fairy-800w.jpg"
        alt="Elva dressed as a fairy">

**srcset** defines the set of images we will allow the browser to choose between, and what size each image is. Each set of image information is separated from the previous one by a comma. For each one, we write:

- An image filename (elva-fairy-480w.jpg)
- A space
- The image's intrinsic width in pixels

**sizes** defines a set of media conditions (ie. screen widths) and indicates what image size would be best to choose, when certain media conditions are true — these are the hints we talked about earlier. In this case, before each comma we write:

- A media condition ((max-width:600px)). (when the viewport width is 600 pixels or less)
- A space
- The width of the slot the image will fill when the media condition is true

With these attributes in place, the browser will:

Look at its device width.
Work out which media condition in the sizes list is the first one to be true.
Look at the slot size given to that media query.
Load the image referenced in the srcset list that has the same size as the slot or, if there isn't one, the first image that is bigger than the chosen slot size.

---

## Things I want to know more about

- Practice in responsive images
- Use of media and video files in document

[Previous Page](https://tomgtaylor.github.io/reading-notes2/class-10)    ||    [Next Page](https://tomgtaylor.github.io/reading-notes2/class-12) <br>

---
[HOME](https://tomgtaylor.github.io/reading-notes2) <br>
