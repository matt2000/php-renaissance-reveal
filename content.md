# PHP Renaissance
## Rebirth of a Diverse Community


Matt Chapman

Sr. Open Source Platforms Engineer

CARD.com

Los Angeles, CA

Note: Tell PHP joke.

#
## Defined

 * Rebirth
 * Renewal
 * Cultural Cross-Polination
 * Unified Diversity

Note: Do this quick

#
## Outline

 * A Personal Story
 * A Technical History
 * A Technical Tour
 * A Look at our Community

Note: The following isn't a real HTML document; this is a code sample, but I
made you this comment because that can be confusing when it's the first code 
block in Markdown.


##
# 2002

    <html>
    <head>

PHP just goes in the HTML file next to the javascript. Why not?
 
    <?php
      $link = mysql_connect('localhost', 'user', 'pass');
      mysql_select_db('testdb', $link);
      // Don't worry, register_globals is on by default until April.
      mysql_query("SELECT * from members WHERE id = " . $id;");
    ?>

Still waiting on the content from marketing...
 
    <p>Under construction!</p>
    </html>

Note: Don't read this.

##
# 2006

    <?php

    function get_data() {
      require_once db_config.inc;
      $db = new PDO('mysql:host=localhost;dbname=testdb;charset=utf8', $config->username, $config->password);
      $db->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
      $db->setAttribute(PDO::ATTR_EMULATE_PREPARES, false);
    ...


##
# 2007

<img src="/img/officespace.gif"/>

##
## Real Estate

<img src="/img/condo.jpg"/>


##
## Home Values vs. Developer Income

<img style="width:47%;" src="/img/GraphA.png"/><span style="width:5%"> </span><img style="width:47%; float: left" src="/img/GraphB.png"/>


Note: Note these graphs don't have the same scale, so please don't get the idea that PHP developers are paying cash for new condos every year. It's a good time, but we're not there yet.

##
## Developer income vs. Average

<img src="/img/GraphA2.png"/>


##
# Footnote

<small>Results not typical; your results may vary. Not intended to treat or<br/> 
prevent any boring or stressful career. May cause rectal bleeding.</small>

Note: So what's the point? This is clealry not a graph of what you can expect to earn
if you start a career in open-source software. This is not a graph about the 
relative stagnation in most sectors of our economy. This graph is the story of
open-source software changing someone's life. We're talking about a real
person, who flourished coming out of the worst recession in a generation.


##
## Changed Lives

<img src="/img/drupalcon.jpg"/>

Note: But this isn't a fully isolated incident. I've been in a room with 
hundreds, if not a thousand, web developers who stood up to say, "My life
was changed by this open-source project." Thank you!

##
## Insanity

<img src="/img/GraphA2.png"/>

Note: It's also a graph about insanity. This isn't normal, and it probably shouldn't 
be! But in the mid-2000s, mortgage bankers were insane, and young home buyers
were insane, and, we can admit it, the PHP world was a little bit insane.


#
# PHP circa 2007

## What's good?
- Fast development cycle.
- Great HTML integration.
- Free, Freer, and Freedom.

##
## What's good about PHP is 
## anyone can do it!
## ~  
## What's bad about PHP is 
## _anyone_ can do it....

Note: Bad & ugly

##
# Terrible Code

    <?php
    namespace Money; 
    
    class Bitcoin { 
     const BITCOIN_NODE = '50.00.00.00'; 
     static private $pending = array(); 
     
     public static function update() { 
       // update all nodes 
       $list = \DB::DAO('Money_Bitcoin_Host')->search(null); 
       foreach($list as $bean) { 
       $bean->Last_Update = \DB::i()->now(); 
       $client = \Controller::Driver('Bitcoin', $bean->Money_Bitcoin_Host__); 

       if (!$client->isValid()) continue; 
      
       $info = $client->getInfo(); 
       if (!$info) { 
       $bean->Status = 'down'; 
       $bean->commit(); 
       continue; 
       } 
       
       $bean->Status = 'up'; 
      
       $bean->commit();

      // If you're actually reading this sample, I should point out that this
      // particular class isn't that terrible. But if you track down a copy of
      // the leaked Mt. Gox source code and read it all, it's a story of
      // betrayal and horror. This is just the omnious establishing scene where
      // the cute kids play unaware of what lurks close by...
      ...


Note: There's a lot of terrible code out there, for Various reasons that we'll discuss. The first reason is, there's a lot of terrible code out there. In every language.


##
## PEAR

 *   PHP Extension and Application Repository
 *   Founded 2000 on the "new" PHP 4
 *   Required root to use properly (WTF?)
 *   Complex process for adding packages
 *   Easy to get wrong

##
## So How does this work?

 * Where do I find code?
    PEAR and, um, forums?
 * How do I get code?
    Paste into your project (or have root)
 * How do I load your code?
    Manual includes
 * How do I load everyone's code?
    Lots of manual includes
 * How can I collaborate on code?
    Sourceforge?
 * Can I exchange code?
    LOLz 

##
# This is why we can't have nice things
-Larry Garfield, PHP-FIG, Drupal.

 * It was hard to share, so everyone built their own.
 * So we didn't get the open-source leverage effect.
 * And 90% of everything is crap anyway.

##
<img src="/img/wordpress.png"/>

Note: 18% of websites.

##
<img src="/img/drupal.png"/>

##
"The average PHP programmer has written </br>
2.5 frameworks in his career, and afterward,<br/>
still doesn't know if needle or haystack comes first."

— Urban legend statistics

Note: Mention Underscore PHP.

##
# Go PHP5.

<img src="/img/forum.png"/>

#
# So What's Changed?
## PHP in 2014

##
# Github

##
# Composer
- PHP packaging system backed by Packagist.org and Github.com

##
# HipHop
- Facebook's Open Sourtime Runtime alternative
- also runs HACK, a backward compatible lanaguge that add optional typing, etc.

##
# Performance

<img src='/img/performance.png'/>


##
# PHP-FIG.org
- Framewok Interoperability Group


Note: PHP done right? Stack-overflow.

#
# What else is hot?

##
# Symfony 2
- Application Framework
- PHP on Rails

##
# Silex, Laravel, Kohana
- Lighter
- Higher or lower level

##
# Phalcon
* Framework in C.

##
# Aura
* No, really, really decoupled.

##
# ReactPHP
* Event Driven Programming
* Inspired by NodeJS & Twisted
* (Not to be confused with ReactJS from FB

##
# Drupal 8 & Backdrop
 * Drupal started in 2001
 * Content Management System
 * 2013 Fork by active community members
 * It's not about OOP

#
# Community
 * What do we want?

##
# Enterprise?

* Red Hat vs Linspire

Note: Not about commercial or not, more about scale. But you can build an OS 
community where any competant contributor can walk into a six-figure job 
anywhere. ProTip: Use an elephant mascot. 


##
# Start-ups?

Note: You should have a really REALLY good reason to NOT use PHP at your 
startup.

##
# Diversity 

Note: Stay-at-home dad, or the enterprise Java developer who's just left her 
mega global company and is ready to launch he own start-up.


#
# Career

##
## Los Angeles is the fastest growing market for tech jobs in the country.
-Some guy I know.

##
# Card.com


#
## Defined

 * Rebirth
 * Renewal
 * Cultural Cross-Polination
 * Unified Diversity

