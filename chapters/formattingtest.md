---
layout: default
title: Chapters
---

# Formatting Test
1. Information [☞](##Information)
2. More Information [☞](https://github.com/dhofu/test_page_structure/new/main/chapters#more-information)
3. Have you considered...? [☞](#have-you-considered)
4. Footnotes ☞
5. Explanation & Step-by-Step

## Information
This is a silly page for me figure out basic interal linking. Ideally, little clickable footnotes that jump around the page.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 
Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
<sup id="footnote1_head">[<a href="#footnote1_foot">1</a>]</sup>
Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
<sup id="footnote2_head">[<a href="#footnote2_foot">2</a>]</sup>

## More Information
In the skeletons of the several breeds, the development of the bones of the face in length and breadth and curvature differs enormously. 
The shape, as well as the breadth and length of the ramus of the lower jaw, varies in a highly remarkable manner. 
The number of the caudal and sacral vertebræ vary; as does the number of the ribs, together with their relative breadth and the presence of processes. 
The size and shape of the apertures in the sternum are highly variable; so is the degree of divergence and relative size of the two arms of the furcula. 
The proportional width of the gape of mouth, the proportional length of the eyelids, of the orifice of the nostrils, of the tongue (not always in strict correlation with the length of beak), the size of the crop and of the upper part of the oesophagus; the development and abortion of the oil-gland; the number of the primary wing and caudal feathers; the relative length of wing and tail to each other and to the body; the relative length of leg and of the feet; the number of scutellæ on the toes, the development of skin between the toes, are all points of structure which are variable.
<sup id="footnote3_head">[<a href="#footnote3_foot">3</a>]</sup>

## Have you considered...?
My dear Lady Lovelace
Mr. Frend’s death (which took place on Sunday Morning)
has made me answer your letter later than I should otherwise have
done. The family are all well, and have looked forward to this termination
for some time. My wife will answer your letter on a part of this.
Number and Magn
. pp. 75, 76. The use of this theorem is shown in what follows.
It proves that any quantity which lies between two others is either one of a
set of mean proportionals between those two, or as near to one as we please.
It is not self evident that the base of Napiers system, as given by himself
is ε or 1 + 1 + 1
2 + · · · as we learn from the modern mode of presenting the
theory. The last sentence in the book (making V a linear unit) would show
that Napier’s notion was to take k in such a manner that x shall
expound [?] 1 + x [‘without’ crossed out] or rather that the smaller x is the more nearly
shall
x expound 1 + x. If this were accurately done
<sup id="footnote4_head">[<a href="#footnote4_foot">4</a>]</sup>

### Footnotes
<sup id="footnote1_foot">[<a href="#footnote1_head">1</a>]</sup> This is the text for footnote 1

<sup id="footnote2_foot">[<a href="#footnote2_head">2</a>]</sup> This is the text for footnote 2

<sup id="footnote3_foot">[<a href="#footnote3_head">3</a>]</sup> This is the text for footnote 3 

<sup id="footnote4_foot">[<a href="#footnote4_head">4</a>]</sup> This is the text for footnote 4

## Explanation

I took all this from the glorious internet, so ordinarily I'd just link to those explanations, except I didn't save them. So you can do a quick internet search, or if you don't want to, read below. (I need a reference for myself if I forget all this)

This is what we will end up with:
The sky is blue.
<sup id="flag">[<a href="#footnote">A</a>]</sup>

Yeah, my eyes glaze over reading that too. 

### Step by step:

<i>Start with a sentence that needs a footnote. (ex. The sky is blue.) </i>

The sky is blue.
[A]

<i>To superscript, use the html tag "sup". </i>

The sky is blue.
<sup>[A]</sup>

<i>We will ultimately want to link back here when we're done, so lets add a little flag ("id") to the superscript to help us find this footnote later. Each flag should be unique across the page, so I'll just show it as () for now </i>

The sky is blue.
(sup id="flag") [A] (/sup)

<i>It should still just display like this, though </i>

The sky is blue.
<sup>[A]</sup>

<i> Now to add the 'link'. The HTML tag for hyperlinks is "a", along with an href="LINK" to tell us where to go. We don't have a flag for where we want to go yet, but lets pretend its called "footnote". </i> 

The sky is blue.
(sup id="flag") [ (a href="#footnote")A(/a) ] (/sup)

The sky is blue.
<sup>[<a href="#footnote">A</a>]</sup>

<i> IMPORTANT: when linking within page, write href="#footnote". Without the # it doesn't work.</i>

<i> And we're done with the sentence! Now lets make the footnote! </i>

[A]This is a footnote

<i> Superscript it, </i>

<sup>[A]</sup> This is a footnote

<i> And from here, we simply repeat what we did before, but flip it! We put the flag id="footnote" in the superscript, and make our hyperlink lead to href="#flag" </i>

<sup id="footnote">[<a href="#flag">A</a>]</sup> This is a footnote.

<i> Tada! Basic html and I feel like such a wizard.</i>

<i> Anyways, if doing just one footnote, saying 'flag' and 'footnote' are fine, but if doing LOTS it probably helps to have a system. I am partial to using NAME_head and NAME_foot, becuase it helps keep track of what connects to what. That might be something to agree on as a class, though. </i>

<i> Anyways, did anyone read all that? </i>






