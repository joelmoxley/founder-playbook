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
* Title: Name of playbook to appear in nav bar
* Playbook: index for playbook
* Description: Description of playbook

Markdown Example:

	---
	Title: Foundational (16)
	Playbook: 1
	Description: ...
	---

## Within Individual Plays
example: 01 – How To Tell Your Story

#### Play index.md

* Title: Name of okay to appear in table of contents
* Play: index for play
* Description: Description of play
* Add section headers with “## Section Name”
* For file listings, each file MUST be written within an ordered or unordered list See below.
* For a file, use the syntax [Display Name](filename.pdf). IMPORTANT: the file path uses a fuzzy search algorithm to find the file closest to the name listed, so the filenames do not have to be exact. However, please note that the filenames cannot be listed with a space in it. I may recommend listing them with underscores or dashes between words.

Unordered lists use asterisks and will appear bulleted.

	* Red
	* Blue
	* Green 

Ordered lists use numbers and will appear numbered.

	1. Red
	2. Blue
	3. Green 

Markdown Example:

	---
	title: How To Tell Your Story
	play: 1
	---

	## Telling A Story

	Telling A Story is about…

	1. [Garage Ventures - Perfecting Your Pitch](01-garage-ventures-perfecting-your-pitch.pdf)
	10-MIN READ II Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
	
	Credit: [Dr. Busybody](http://www.busybody.com), [Dr. Soandso](http://www.soandso.com)
	
	2. [a - David Merkoski - Telling Your Story](02-a-david-merkoski-telling-your-story.pdf)
	5-MIN READ II Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
	3. [b - David Merkoski - Telling Your Story](02-b-david-merkoski-telling-your-story.webloc)
	30-MIN READ II Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.


	## Design Thinking

	Design Thinking is about…

	1. [Stanford d.school - Design Thinking Method Guide](01-stanford-d.school-design-thinking-method-guide.pdf)
	15-MIN READ II Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
	Credit: [Mr. Alchemy](http://www.alchemy.com)
	2. [Stanford d.school - Design Thinking Process Mode Guide](02-stanford-d.school-design-thinking-process-mode-guide.pdf)
	25-MIN READ II Lorem ipsum dolor sit amet, consectetur adipiscing elit.


## General Syntax:

	# Header 2
	## Header 2
	[Test Link](test_link.pdf)   text_link.pdf CANNOT have spaces. It’s ok if the filename itself has spaces, just list it with underscores or dashes and it will find the correct file.
