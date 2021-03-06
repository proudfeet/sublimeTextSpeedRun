#Sublime Text Speed-Run

Here's a quick document to get you up and running and writing code, along with some tips that should speed up your workflow drastically.

Your text editor is your most cherished and heavily used tool for development, so it makes sense that you would want your editor to be optimized in such a way that would help you do your job. My personal recommendation with regard to text editor is [Sublime Text](http://www.sublimetext.com), which I strongly recommend you download.

Out of the box, Sublime, while it is a great editor as is, is not at it's full potential. Let's go ahead and install Package Control so we can make Sublime more useful for ourselves. Head on over to [the instructions for installing Package Control](https://sublime.wbond.net/installation) and follow the directions exactly, depending on which version (2 or 3) of Sublime that you are using. After you are done installing Package Control, you may (most likely will) need to restart Sublime for Package Control to take effect.

So why am I so adamant about installing Package Control, anyways? Package Control allows us to add packages (duh) that extend the functionality of Sublime by a mile. One of my most used and favourite packages is on called [Emmet](http://www.emmet.io), which I'm going to guide you through the installation of now.

##Installing packages
- First, we're going to tell Sublime that we want to access Package Control. To do this you can either click on `Sublime Text -> Preferences -> Package Control`
- In the interest of saving time, you can also press `super(command on Mac, window key on PC) + shift + p`
- From here, type in "install package". As you type, you'll notice that the search auto-completes for you and you can simply press enter to select this option
- Now, we have access to all the packages available on Sublime. As mentioned before, the one we're specifically looking for right now is called Emmet, so go ahead and start typing that into the search bar (again, you'll notice the auto-complete feature kicking in
- Go ahead and press enter on Emmet to install the package, and once again, you'll probably need to re-start Sublime for the package to take effect

Congrats, you've now installed your first package in Sublime Text!

##Emmet
Now, onto actually using Emmet. Emmet is a plugin that allows you to speed up your actual time spent writing code by a huge factor. It essentially allows you to scaffold your code quite quickly. Let's start with a very simple example.

- Normally, when we want to target a div with a class of wrapper in our CSS, we would write `div.wrapper`, right?
- What Emmet allows us to do is to do the same thing, but with our HTML which is triggered via the tab key, as seen below
- ![Simple example of Emmets functionality](http://i.gyazo.com/9b9e058fa9f314cebc2fd375691f9891.gif)
- While this might not seem like the biggest deal right now, it can come in super handy when you're writing a bunch of nested elements (again, using the same syntax as you would with CSS), as seen below
- ![Example of using emmet with nested elements](http://i.gyazo.com/901a595c8237905356488b3cda774562.gif)
- Pretty awesome, right? The best part about this is that you can now simply press tab and Emmet should allow you to simply tab through the areas of the tags that need to be filled out such as the href and the actual content of the link
- You may have noticed that I added multiple classes to the list items, by simply adding another class (again, as you would in CSS) to the list item before scaffolding
- You may have also noticed that on the second class of the list item before scaffolding had a dollar sign at the end. When expanded, it gave each element a class of `menu-item[number]` because Emmet is, behind the scenes, iterating through a loop and generating the numbers for you
- If you're super crafty, you could even get Emmet to scaffold a simple web page for you in a few keystrokes
- ![Emmet scaffolding entire page](http://i.gyazo.com/91af5d6ec956468b626172edaa2b3da1.gif)
- There's lots of tricks to Emmet and we've only scratched the surface. While it might feel weird at first, I can promise you that if you spend the time to train yourself to use Emmet properly, it can save you hours of development time. If you ever need a refresher, feel free to check out the [Emmet cheat sheet](http://docs.emmet.io/cheat-sheet/)
- Above all, using Emmmet can help you cut down on errors - it's very easy to miss a closing tag here, a quotation mark there, and Emmet helps you reduce those easily preventable mechanical errors

##Getting set up
Alright, enough talk about writing code, let's actually get to writing some code. Go ahead and create two new files either by clicking `File -> New File` or keyboard shortcut `cmnd/window + N`. You'll notice that when you first create these files, the syntax of each is set to `Plain Text` by default (viewable in the very bottom right hand corner). While you can still write both HTML and CSS in a plain text file, it will be much easier due to syntax highlighting etc. if you set the syntax of the document to whatever kind of code we're going to write. 

There are three ways of doing this, the first being clicking on the very bottom right corner that says `Plain Text` to show all the possible options. From this, choose HTML, CSS, or whatever language you happen to be writing.

The second way is quite similar, except that this time we're going to go to `View -> Syntax` and then select whatever syntax we'd like to see for our document.

The third, and my personal favourite way is to use Sublime's "fuzzy search" using the command pallet. To use this, press `cmnd/window + shift + p`. From here, start typing `Set Syntax: HTML`. As you're typing this, you'll notice that more options become available. You can let Sublime do some of the work for you, but simply typing `ssht` and it should autocomplete to the most relevant thing, in this case `Set Syntax: HTML`. If we were writing a Python file, we could just as easily search `sspy` and would be able to set the syntax of our document to Python.

If you ever find yourself lacking a certain syntax highlighting (for instance, you may find that you need Sass, Less, or Stylus syntax highlighting), you can again download these through package control. Simply press `cmnd/windows + shift + p` and type in `Package Control: Install Package` (use fuzzy search by just typing `install`) and then search for your desired syntax.

Go ahead and create a simple web page in your HTML file, remembering to link the CSS in the head of your HTML document (**tip**: put Emmet to use by simply typing `link` and pressing your `tab` key, and a link tag should be ready to go, just type in the name of your file in the `href` attribute). Open up your files in your editor. Right now, your two files should be in two tabs in a single pane. While this is alright, I'm personally a fan of having two panes open, particularly when editing CSS so I can reference my HTML easily. To do this, go to `View -> Layout -> Columns:2`, feel free to stick to one pane or use as many panes as you like. You can, alternatively, use the keyboard shortcut `cmnd/windows + option/alt + [number of desired panes]`. Drag your desired files into the second pane. You should now have something like looks like this
![Sublime Text with two panes](images/sublimeTwoPanes.png)

##Small things that help you out big time
There's a number of small things that I use in Sublime that I find help me out big time in the long run. These things might seem trivial now, but when you're knee-deep in code anything helps

###Changing themes
Personally, I'm a huge fan of dark themes in text editors - I spend at a very minimum 8 hours a day looking at a screen, and I'd like to do everything I can to maintain my (already poor) eye health. To change your theme, click `Sublime Text -> Preferences -> Color Scheme -> Color Scheme - Default` and pick a theme from there. If you'd like to download a custom theme, bring up your package control search and look for themes you'd like to install. Scotch.io has a great write-up on the [best Sublime Text themes of 2014](http://scotch.io/bar-talk/the-best-sublime-text-3-themes-of-2014) that should serve as a great starting point.

To enable your custom theme, follow the same steps as above, but instead going to `Sublime Text -> Preferences -> Color Scheme` and selecting your desired theme from there.

###Editor preferences
Sublime allows you to do a lot of customization through the preferences files. To see a complete list of all the available options, go to `Sublime Text -> Preferences -> Settings - Default`, but don't modify any of the code in this file. Any settings you'd like to change should go into `Sublime Text -> Preferences -> Settings - User`. Given that the code you'll be writing is JSON, all your preferences you're entering must fall between the two curly-braces, you must use quotation marks where appropriate, and all of the key and value pairs (save for the very last one), **must** be followed by a comma. I've prepared some code of preferences I think are very helpful, which you can pop right into your User preferences file.

```
{	
	"bold_folder_labels": true,
	"caret_style": "wide",
	"font_size": 14,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"line_padding_bottom": 1,
	"line_padding_top": 1,
	"match_brackets": true,
	"match_brackets_angle": true,
	"match_brackets_braces": true,
	"match_brackets_content": true,
	"match_brackets_square": true,
	"open_files_in_new_window": false,
	"scroll_past_end": true,
	"show_full_path": true,
	"spell_check": true,
	"word_wrap": true
}
```

A note about word wrap: you may want to disable this feature if working with a language that renders whitespace

###Working with multiple cursors
Sublime Text supports multiple cursors, which we should definitely take advantage of when applicable. To simply add another cursor to our document, simply click where you would like the first cursor to appear, hold `cmnd/control` and click where you would like your next cursor to appear, repeat as many times as necessary and type as normal. 

If you have some markup that's aligned you'd like to enter a cursor into, you can expedite this process by clicking and holding where you'd like the first cursor to appear, holding `cmnd/ctrl + alt/option` and dragging your mouse up or down to where you would like other cursors to appear.

###Keyboard shortcuts
Keyboard shortcuts are a great way to not only save yourself some time - but also save yourself from developing carpal tunnel syndrome. The less time you spend switching between mouse and keyboard the better

If there's certain words or strings that you'd like to select across a document, highlight your desired string and press `cmnd/control + d` to go to the next instance of that string in your document. If there's a particular instance of that word that you would like to skip (i.e. searching for `some` would also select the `some` in `awesome`), simply press `cmnd/ctrl + k`.

If you come across a scenario where you'd like to wrap some text in a tag, such as when a client gives you a piece of copy that you copy and paste into your document press `ctrl + shift + w` to wrap your selected text in a tag. By default, Sublime will wrap your text in a `<p>` tag, but not to worry - if we want to change it to a `div`, start typing and both the opening and closing tag will be updated. To add a class, press space and start typing and Sublime will drop the second cursor in the closing tag for you.

The above shortcut is dangerously easy to confuse with `cmnd/window + w`, which automatically closes the window without giving you the option to save your work. I hardly use ever *mean* to use that feature, so I've re-mapped `cmnd/window + w` to wrap tag for me. To do this, go to `Sublime Text -> Preferences -> Key Bindings - User` and add `{ "keys": ["super+w"], "command": "insert_snippet", "args": { "name": "Packages/XML/long-tag.sublime-snippet" } }` in between the two square brackets. Give it a save, restart Sublime, and you should be on your way to wrapping bliss.

If you'd like to add more custom key bindings, your `Key Bindings - User` is the place to do it.

####Wrapping tags on hardcore mode
Sometimes you have a small piece of text that you'd like to wrap in a series of nested tags. For example, you might have `This is some text I need to wrap`, in a link, in an h1, in the header within the wrapper div. Obviously, we could use Emmet to do some of this scaffolding for us by typing `div.wrapper>header>h1>a + tab`, copying our text and then moving it into the desired place, but if we can get our editor to do a bit of the work *for us* then when wouldn't we, right?

To do what I call wrapping in "hardcore mode" (I wish this was a thing), highlight the text you'd like to wrap. Next, press `ctrl + w`, and you should see a small dialog box open up at the bottom of your editor. From here, we can use our Emmet tricks to do some of the wrapping for us. So to achieve:
```
<div class="wrapper">
	<header>
		<h1><a href="http://www.google.ca">This is some text I need to wrap</a></h1>
	</header>
</div>
```

Enter in `.wrapper>header>h1>a[href="http://www.google.ca"]` and hit enter. Congrats, you're hardcore now.


You may find yourself needing to move code in and around your document as you get further along in your project. As we all know, maintaining neat code is a huge portion of having a maintainable, clean code-base. It's a huge drag when you go to move some code around only to botch your indentation you worked so hard for. Fear not, there is a way around this! If you're pasting code, when you're going to paste, instead of just pressing `cmnd/ctrl + v`, pressing `cmnd/ctrl + shift + v` will paste with correct indentation (as correct as possible, it is a machine, after all). 

If you're moving code around and your indentation goes belly-up as a result, or if you've already pasted without throwing the ol' `shift` in there, there is still one last hope: highlight the text you'd like to re-indent, and go to `Edit -> Line -> Reindent`, which should do the trick for you.

As I mentioned before, we can make custom key bindings for the things we'd like to automate, so let's go ahead and do that for our re-indentation. Head back over to your `Key Bindings - User` file, and paste in `{ "keys": ["super+option+r"], "command": "reindent"}` after our key binding for our wrap-tag function, making sure to add a comma after the last curly brace in the wrap key binding. Our `Key Bindings - User` file should now look like this 

```
[
	{ "keys": ["super+w"], "command": "insert_snippet", "args": { "name": "Packages/XML/long-tag.sublime-snippet" } },
	{ "keys": ["super+option+r"], "command": "reindent"} 
]
```

This will re-map `cmnd/window + option/alt + r` to re-indent our code. Give it a save, a restart, and get to re-indenting!

You can initiate a global search in Sublime by pressing `cmnd/window + p`, which can be super handy when you're looking for one specific file within a huge project. 

##Snippets
I think by now you realize that I'm big on cutting down on writing code that you don't have to, hence my love of Emmet. Another great feature of Sublime Text is the ability to create "snippets", which are little bits of code that you can re-use. What Emmet is doing is essentially giving you access to a host of snippets that the Emmet team noticed that they were using frequently, and we can do the same. To create a snippet click on `Tools -> New Snippet`. This should bring you to a new tab that already has some code written on it. Let's take a look to make sense of it while making our own snippet.


###Making our own snippets
- At first, you should see a screen that looks like this:
![Start of Sublime Text snippet](images/snippetStart.png)
- It may seem like a pretty confusing and discouraging starting point, but it's actually not so bad once you make sense of it
- The code you see in between `CDATA[` and `]` is where all the code of our snippet will go
- The code you see such as `${1:this}` is where tab indexes begin. Tab indexes are usually words within your snippet that can change easily depending on the context. In this example, once our snippet is called (which we will get to) the cursor will appear there first, and the word `this` will appear, but also be editable
- The code (or lack of, in this particular instance) between `<tabTrigger` and `</tabTrigger>` are the keywords we'll use to call our snippets, which will be called via the tab key
- Let's go ahead and uncomment the line with our tabTrigger code on it (feel free to use the keyboard shortcut `cmnd/windows + /`) and insert the word we would like to trigger our snippet. For this example, please use `placeholdit`
- ![Starter for first custom snippet](images/placeHoldStart.png)
- Now, let's edit the actual portion of the code that will be generated with our tab trigger. In this example, let's start by making our snippet `http://www.placehold.it/200/200`
- ![Editing the generated code in a custom snippet](images/placeHoldSecondStep.png)
- At this point we could stop here and call it a day on this snippet, but I think it's reasonable to assume that we will not **always** want to generate a placeholder image that's 200x200 pixels, and since we can save time on this by editing our snippet, I think that we should
- As I mentioned before, we can set tab indexes on editable portions of code within our snippets to have them better suit our needs
- For this example, we'll set two tab indexes on the pixel value portions of our snippet, starting with the first dimension, and ending on the second dimension
- To do this, envelope the first `200` in a pair of curly braces and precede them with a `$` so your snippet code now looks like `http://www.placehold.it/${200}/200`
- To make this the first tab index, place a `1:` before `200`, so that your code now looks like `http://www.placehold.it/${1:200}/200`
- Repeat the above steps on the second pixel value, this time replacing `1:` with `2:` to make this value the second editable tab index, your code should now look like this `http://www.placehold.it/${1:200}/${2:200}`
- At this point, we're done with our snippet for now. The next step is to save it, which follows a very specific format
- Go ahead and save this snippet, the snippet must be saved in `Sublime Text [version] -> Packages -> User` (which you computer will most likely bring you to automatically) and **must** be saved with a `.sublime-snippet` extension, so in our example, let's save our snippet as `placeholdit.sublime-snippet`
- Head over to an HTML file, and go ahead an use your snippet wherever appropriate
- ![Using your custom snippet](http://i.gyazo.com/c7fec0a36fef9c457280bfc5c15495eb.gif)
- A quick note about snippets: certain characters will throw your snippet effectively down the tubes, such as `$`. To circumvent this, you can escape these characters by preceeding them with a backslash
	- Note that this does not apply to tab indexes within your snippet, which must follow the specific syntax of `${[number]:[word]}`
- As an example: `$(".box").click(function(){});` would not work as a snippet. However, by simply adding a `\` before the `$` so that our snippet now looks like `\$(".box")`

##We need to talk about Emmet...
While Emmet is a great tool for scaffolding code quickly, there are a few things that I had always *wished* it would have. For example, I noticed that image tags wouldn't come with alt tags, which I would then have to manually add. It's not the hugest inconvenience, but the point of these tools is to automate these kinds of things, so it was always nagging at me in the back of my head.

The obvious solution would be to create my own image tag snippet, and use that instead. The problem with that, is that it's both redundant and it can also create issues with the snippet not triggering at all (this can sometimes happen when you're trying to override Emmet snippets with your own).

The next obvious solution would be to edit the Emmet snippets themselves, which seems like the most practical solution. To do this, we're going to need to turn to terminal. It's also going to help to create a symlink for Sublime in our terminal, [a great blog post for how to do so can be found here by my friend Wisam](http://wzaghal.wordpress.com/2014/05/19/how-to-launch-sublime-text-from-terminal/).

Once you've got that set up, head to your terminal and run `subl /Library/"Application Support"/"Sublime Text [version]"/Packages/Emmet/emmet/snippets.json`, which should open this file up in your editor.

This is where, if you'd like to, you should make all your changes to your existing Emmet snippets. The syntax for these follows exactly the same syntax as when we made our own custom snippets beforehand, the only difference being that we can set multiple things as triggers. For example, we can see that on line 648 we have `a:mail` to trigger `<a href=\"mailto:|\"`, but we can make this more efficient by setting it simply to `mail`. 

I'm hesitant to completely remove the functionality of `a:mail`, because something else in your `snippet.json` file could be dependent upon it. So to circumvent this, we're going to assign multiple triggers to it, which we do by simply adding `|[alternative trigger]`. Now, line 648 should look like `"a:mail|mail": "<a href=\"mailto:|\">",`