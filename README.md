# badlybluestocking
Hi Freya, this will be your website once it is up and running! :D

Okay, now the website is functioning, so it is now possible for you to start writing x

## 0: Using this guide

Unfortunately, when I was writing this guide, I didn't realise that all the very important symbols I was using wouldn't actually show up. This sucks.
So the very first thing to do it to open this guide in edit mode, so you can read the very important symbols, or else this guide is literally useless.

In the top-right corner of this guide, there is a pencil icon. Click it.
You should now be on a page where you can still read the guide... but it looks more code-y and crappy.
Fortunately, it has all the important symbols you need in order to understand what to do.
Enjoy!

## 1: Writing a blog post

The first, and easiest thing to do is to write a blog post (just text).

Click the link in the list above: index.html (in a new tab, so you can keep referring to this).
All of the code for your website's main (and currently only) page will then appear in a big white box.
At the top-right corner of the box there are 3 icons, including a pencil. Click on the pencil.
Now you are ready to edit!

Scroll down to the first sequence of lorem ipsums. You can see that I've written "<p>", "this is an example of a post", many "lorem ipsum"s and then "I hope this works", followed by "</p>".
<p> means the start of the paragraph, and </p> means the end of the paragraph. Anything between them comes up as text.
As a more general note, <x> is the start of x and </x> is the end, where x can be anything. x is most likely to be "p", "div", "center" etc.

Delete everything within the paragraph and the start writing! x

Writing text in html is really easy. Once you are between <p> and </p>, it works exactly the same as MS Word.
There is only one difference. Pressing enter will create a new line on the editor (which you are currently on), but will not create a new line on the website.
For this, you need <br>, the BReak element. Putting <br> will create a new line in your paragraph on the website.
If you put <br><br>, you can create a new paragraph.
The more <br>s you put, the bigger the gap between paragraphs. 2 will be fine unless you deliberately want a larger break.

Hooray! That's your first post!

Scroll to the bottom of the page.
A greyed-out box will say "Update index.html". That is your commit summary. You can leave it as it is, or call it whatever you want.
This time, call it "Post 1".

Then click on the green "Commit changes" button.

The page will now look like it did before you started editing. 
Click on "code" (it has an orange underline) to get back to the main page.
Finally, wait up until 2 minutes, and then refresh https://badlybluestocking.github.io, for your first post to appear!
I have put in 3 lorem ipsum boxes in case you would like to make another post or two x

## 2: Playing about with text

There are different ways to format text within a paragraph to make it more exciting:

<b> bold </b>
<i> italic </i>
<s> strikethrough </s>
<u> underline </u>
<sup> superscript </sup>
<sub> subscript </sub>
<big> bigger text </big>
<big><big> even bigger text etc </big></big>
<small> smaller text </small>
<small><small> even smaller text </small></small>
<strong> This is currently set to make the text neon green </strong>

You can combine any of these in any combination:

<b><i><u><big><strong> bold italic underlined bigger neon green text </strong></big></u></i></b>

Just make sure you close each setting with the appropriate </x>, or else all the rest of the text on the page will be turned x!

## 3: Creating a new post

I have only included 3 posts on the website, so to make a 4th one, you'll have to add it yourself.

The <p> paragraph </p> of each post is itself contained within <div class="post"> a div element </div>. 
The div element is arguably the bread and butter of html. James uses hundreds of them before I come and cull them.
As much as overuse of divs annoy me, they are a very useful tool. They are basically a box. You give the box a name (these are called "post") and once named, you can make the box look however you want ("post" is set to be white, but semi-transparent, have a width of 60%, a little padding, and curved corners).
So on their own, when you just have these individual "post" boxes lined up on the page (in a sequence of individual blog posts), they are really useful. But for the love of God, please don't do what James does and put divs inside divs inside divs inside.... - it is the internet's equivalent of pass the parcel - boxes within boxes within boxes.

To make a new post, copy the first entire div element (an entire post, including <div class="post"> and </div>), and also copy the <br><br> underneath it. The <br><br> here is to separate the posts from fusing with each other.
Simply paste what you copied above the first post (and below the <a href=....></a>). 
  
Yay! You now have a 4th post!
Just delete everything within the paragraph and get writing! x

## 4: Images

There are already some images on the website, but the chances are that you'll want to add more.
Luckily, that is easy.

On the main code menu, there is a link to a "photos" folder. Click on it.
It will now take you to the list of all the photos on your website. In the top right corner there is an "upload files" button. Clicking on it will allow you to choose your files from your computer to add to the website. Once you've selected all of them, you can write a commit summary if you want, before clicking "commit changes".
Your new photos are now on the server.

(NB! If your photos are already online, then adding photos to the website is even easier - ignore the above step)

Next, go onto index.html and start editing.
Here you can put in the code for your new photo to appear.
You need to use the <img> tag.

<img> is another easy tag to use. You can put it pretty much anywhere - outside of the divs, inside a div, or even inside a paragraph!
However, it is the first multi-argument tag you will be using (apart from <div class="post">), so be careful.

The completed tag will look something like this: <img src="./photos/pic.jpg" align="right" width="20%" class="name">

"src" is the source of the photo. If you have just uploaded your new photo to the server from your computer, then replace "pic.jpg" with the picture's name.
If you got the photo from the internet, then replace the whole address within the speech marks with the URL of the photo.

"align" and "width" are pretty self-explantory - "align" will align your photo to the left or right (center is default - if you want your photo to be central, then omit "align" entirely), and "width" specifies the width of your photo.

Finally "class" allows you to name the photo. This is entirely optional. You don't have to.
If you name the photo, make sure to pick a unique name. If 2 things have the same name on the website, then this can cause major problems.

Once you are done, write a commit summary at the bottom and commit changes.
Now your image is on the website! Hooray! Wait a few minutes before refreshing https://badlybluestocking.github.io, and it will appear!

## 5: Hyperlinks

I will briefly mention how to hyperlink things, which is another easy task.

This is the hyperlink tag: <a href="">hyperlink</a>
Unlike img, but like most other tags, you must close this tag with </a> !

href is the URL of the item you are linking to. Just paste in the URL between the speech marks.

Whatever text is between <a href=""> and </a> will come up as blue and underlined (although I think it may be set to green on this website). If you click on that text on the website, it will function as a hyperlink.
But it doesn't have to be text! There is an example towards the top of index.html of an image being hyperlinked to your Tumblr account. Just put <a href="..."><img src="..." align="..." width="..."></a> to achieve this effect.
<a></a> is really powerful - you can put pretty much anything in the middle and hyperlink it - even entire divs! (Don't do that though - that'd be silly).

The URL you put for href can be anything you like from the entire internet, not just this website. You can link to Tumblr, Facebook, Twitter, Instagram, Wikipedia etc.

## 6: TBD

That's all I'm going to write for the moment - hopefully that was easy to follow x
I will probably write more at some point, but these 5 posts are all you really need for the moment - there isn't a huge variation of code on a blog.
For the moment, I will take care of all the css and any more advanced html than the stuff written above.
In future, I will tell you how to split the blog into different pages (initially like your tumblr, but later into categories like NT (and eventually into categories like NT, each with multiple pages like your tumblr), but that is a bit more fiddly, and I have to add some navigation buttons/a menu first.

Either way, I hope you really enjoy your blog - no greedy data-sucking company is monitoring this XD

I love you x
