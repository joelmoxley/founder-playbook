# Founders Playbook Markdown Instructions


## Within Main Directory:

#### Main index.md

Use this to change the text on the home page. Example:

    ---
    Title: Founder Playbook
    ---
    
    # Home Page
    Example home page content


* Main footer.md – Markdown for the lower grey area. Edit that content here.
* Main 404.md – Text used for the Error 404 page
* img folder – contains all image assets for the playbook

## Within Individual Playbooks
example: I. Foundational

#### Playbook index.md 
Use this to change the content at the top of a playbook.

Markdown Example:

	This playbook is great!

## Within Individual Plays
example: 01 – How To Tell Your Story

For each play, you can have an index.md (header) or footer.md (footer), which will appear above and below the files for that play. Use index.md to add content that explains the play. Use footer.md to add the associated Network/Experts listing. Details for both are below:

#### Play index.md

Markdown Example:

	Check out this play!

#### Play footer.md
Use this markdown to add Network/Experts to the bottom of the play page.

Markdown Example:

	## Network / Experts

	* ![](https://media.licdn.com/mpr/mpr/shrinknp_400_400/AAEAAQAAAAAAAAQOAAAAJDdkZDZmNTY1LWQ5YjMtNGVkYS1hM2RjLTFiNDAxNzljMjQxZg.jpg)
	    [Justin Bessant](http://example.com)
	    Development
	    Engineer at Zero Mass
	* ![](https://media.licdn.com/mpr/mpr/shrinknp_400_400/AAEAAQAAAAAAAAQOAAAAJDdkZDZmNTY1LWQ5YjMtNGVkYS1hM2RjLTFiNDAxNzljMjQxZg.jpg)
	    [Nicholas Walrod](http://example.com)
	    3x5 Partners - Managing Director

## For Individual Files

All markdowns for individual files are stored within the "md" folder within a play. Each markdown should have 1 corresponding markdown file with (".md") appended to the end of the name. For example

	../01 - How To Tell Your Story/01 - Content - Telling A Story/01 - Garage Ventures - Perfecting Your Pitch.pdf
	../01 - How To Tell Your Story/01 - Content - Telling A Story/02 - a - David Merkoski - Telling Your Story.pdf
	../01 - How To Tell Your Story/01 - Content - Telling A Story/03 - Nancy Duarte - Greatest Communicators.webloc
	
	../01 - How To Tell Your Story/01 - Content - Telling A Story/md/01 - Garage Ventures - Perfecting Your Pitch.pdf.md
	../01 - How To Tell Your Story/01 - Content - Telling A Story/md/02 - a - David Merkoski - Telling Your Story.pdf.md
	../01 - How To Tell Your Story/01 - Content - Telling A Story/md/03 - Nancy Duarte - Greatest Communicators.webloc.md

These files can be manually added or edited within github, or you can use the "pencil" icon next to a file within the UI to assure you have the correct Markdown file path.

File Markdowns should be used:
1. To add a short description of each file. This will appear below the file within the playbook.
2. To add credit links. Must begin with "Credit: "
3. To add file content to be used by the search. This content should be added below the "{! SEARCH-CONTENT: !}" tag. Everything below this tag will be hidden from the user.

Markdown Example:

	15 MIN READ || Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

	Credit: [Garage Venture Technologies](http://garage.com)

	{! SEARCH-CONTENT: !}
	Perfecting Your Pitch

	By Garage Technology Ventures

	Endless articles,  books,  and  blogs  have  been  written  on  the  topic  of  business plan  presentations  and  pitching  to  investors...

## General Syntax:

Headers:

	# Header 2
	## Header 2

Links: Please Note, text_link.pdf CANNOT have spaces. It’s ok if the filename itself has spaces, just list it with underscores or dashes and it will find the correct file.

	[Test Link](test_link.pdf)   
	
Lists:
Unordered lists use asterisks and will appear bulleted.

	* Red
	* Blue
	* Green 
	
Ordered lists use numbers and will appear numbered.

	1. Red
	2. Blue
	3. Green 

## Dev notes:

	* UX upgrade / overhaul
		* Focus on mobile
		* Every click and gesture creates an immediate user action, even if things need to be loading in background
		* Design queues to swipe on mobile and/or paddle left / right on desktop
	* Create permalink landing page for each file
		* Shareable url
		* Big button to access the file
		* Description section (with the edit pen to markdown moved to here)
		* Search text section (indexable and appears long tail google searches)
	* Next gen playbook displays
		* Replace edit pen icon with the permalink icon
		* Automaticaly calculate read time by the word count of the markdown file (especially search text)
