# Finding appropriate sources

Your paper will be based on recent peer reviewed computer science research literature. We require you to have at least three reasonably recent peer reviewed sources as key sources of your paper. 

It is essential that you use sources that inform you about the topic of your paper in a way that you can understand and summarize in your paper and your presentation. The topic of your paper is ultimately determined by your sources. If the source papers that you are trying to use are too complex or not detailed enough or poorly written, writing your own paper based on these sources would be very challenging and may be frustrating. Thus, choosing good sources at an appropriate level is one of the keys to writing a good senior seminar paper. 

## Finding sources

*Peer reviewed* computer science literature means papers that were published in computer science journals or proceedings of computer science conferences or workshops where publications are selected based on reviews by experts in the field. This writeup explains peer review process: [Meet Science: What is "peer review"?](http://boingboing.net/2011/04/22/meet-science-what-is.html). 

## Guidelines for sources for your paper

While the general requirement is to have at least three fairly recent published peer-reviewed sources, the specifics of these requirements depend on your topic: 

**Recent sources** For an active area and a sufficiently general topic (e.g. machine learning or network security) we would expect that all your primary sources are published within the last 3-4 years. If your topic is more specific and/or slower developing (e.g. applications of machine learning to medical records or assistive technology for middle school teachers), you might not be able to find all sources within the last 3-4 years. In this case it's ok to have one more recent source (within 3-4 years) and the other two be somewhat older. 
<br />
It is up to the student to search for sources and to discuss with their adviser and the senior seminar instructor what is available. If no new sources are available, but the topic is interesting, we may suggest widening the topic or we may be ok with the student using somewhat older sources.

Some senior seminar papers are survey papers and cover more than three sources. For instance, see[Concurrent Compaction in JVM Garbage Collection by Jacob Opdahl](../seminars/Fall2015/Opdahl.pdf) ([Fall 2015](../seminars/Fall2015)).

We also want to make sure that you are presenting a reasonably complete picture of the state of the art in a specific area. Thus your three primary sources shouldn't all come from the same author or group of authors. 

**Primary vs supplementary sources**
Primary sources are the ones that provide information for the core of your paper. Your paper needs to clearly explain the methods and the results presented in your primary sources in a way that's understandable to students at the Data Structures level. 

In order to better understand methods used in your paper you are likely to use supplementary sources: papers that the primary sources are building upon, textbooks, technical reports, wikipedia articles, talks and blog posts by researchers explaining the concepts, etc. Some of these materials may be peer reviewed, and some wouldn't be. Make sure they are trustworthy. You need to cite them in your paper (we discuss proper citing later). 

**Using your sources**
Typically your three sources cover the same topic from different angles. **TO DO: mention Max's paper, Kristin's**

**To Do: mention Lemmon's paper**

### Journals vs conferences vs workshops

### How to find peer reviewed sources

Most senior seminar students start with some idea of what their topics of interest are. However, this idea may be vague, or it you may be choosing between several different areas of interest, or you may not know if a topic you are interested in is appropriate for senior seminar. That's ok. In the first 3-4 weeks your goal is to find good sources, narrow down your topic, and discuss your options and findings with your adviser, to make sure that you have a solid topic and a solid set of good peer reviewed sources. 

Most peer reviewed sources in CS are indexed in ACM Digital library and/or in IEEE Xplore database. However, these databases may not be the best starting point for looking. Google scholar may be a better starting point.  

#### Google scholar vs CS databases

You probably would start by searching on key terms of your topic in google scholar, and then proceed to the CS  databases for more detailed information. 

Since google scholar and CS databases provide different benefits, you are likely to use some combination of both. Here are strength and weaknesses of each approach. 

* CS databases reference papers by keywords used by experts in the field. If you are trying to find papers knowing less formal keywords, google scholar is a better source. For instance, common terms such as *computer graphics* or *compiler* would give you better results in google scholar. 
* CS databases list mostly peer reviewed sources (with some exceptions, such as invited talks and textbooks which are not peer reviewed). Google scholar lists everything that looks like scholarly work. Examples of non-reviewed work that comes up on Google scholar are technical reports, drafts that never got published, course work by students, etc.  
* Google scholar tends to give preference to more recent materials. This may be a good thing since you are looking for recent papers, but may also be problematic if you need background work on a subject.    
* Google scholar indexes papers in all areas of science, not just CS. Be careful with common search terms, they may mean something entirely different in another area of science (e.g. *mutation*). CS  databases list only CS-related papers (although IEEE also includes computer engineering). 
* Both google scholar and CS databases cross-reference papers by citation, i.e. you can find papers that cite the one you are looking at, as well as the ones that are cited in it. This may be useful for finding related work. Both also allow you to find other work by a given author. 
* CS databases also list papers by conferences or journals. This may be useful if you are interested in a specific topic (say, computer graphics) and would like to see what was published in this area in the last few years. 
* CS databases tend to be US-centered. Papers published in European, Asian, or Australian venues may not be listed in these databases. Google scholar may be a better source. 
* Many conferences and journals do not allow authors to have full texts of their papers in public domain. UMM has access to full texts of most of such papers in ACM digital library and IEEE Xplore. Thus once you find a potentially interesting paper in google scholar, you might want to look at its page in ACM digital library (log in through UMM) to read the abstract and see its full text.  
* ACM digital library has information about acceptance rates for most conferences and workshops. This is useful for evaluating quality of sources. 

Taking advantage of the strength of both approaches, here is how you can find sources for a topic:

* You may start by looking by specific keywords in google scholar and/or by looking at specific conference proceedings in ACM digital library or IEEE Xplore. 
* If you are using google scholar, make sure that your paper is a peer-reviewed source: it must appear in conference or workshop proceedings or a journal. 
* If a paper title looks interesting, read the abstract.
* If this paper looks interesting and relevant based on the abstract, make a note of it and look for related work, either in similar conferences, or by keywords in google scholar. 
* You may use citations in the paper and "cited by" to find related work. In particular, for recent work you may do a "down and up" citation search: look at papers cited in your paper, find a source that seems to be fundamental to the paper, and then look at papers that cite this source. 
* Once you have identified a few sources, try to find their full texts in a CS database (ACM or IEEE). 

### How to find good quality sources

Once you have found full texts, you need to try to evaluate the quality of your sources. It's a tricky process, but here are some things to take into account:

* The venue where the paper was published:
   * Conferences and workshops often list their acceptance rate in the *Publication* tab in the paper page in ACM digital library. What's considered reasonable for acceptance rates varies between different fields in CS and depends on how specialized the conference or a workshop is (more specialized ones tend to have higher acceptance rates, that's ok). However, an acceptance rate over 50% is usually not an indication of rigorous review (more than half of submitted work is accepted), and below 25% is usually very good. 
   * Another indication of rigor in review is the length of the review process: if a conference gives 2 months or more to review a papers, this indicates rigor. A month or less is usually not enough for thorough review. A rebuttal of reviewers' feedback is usually a positive sign. Information about the review process is included in the Call for Papers (CFP) for the conference. It is roughly the same every year, so you can find the most recent one. 
   * Journals list their review process on their web site (in submission information). Note that review by editors is not considered peer review. More specific journals match a paper with experts in closer areas, and thus are generally more rigorous.  <br /> Watch out for invited papers, and also make sure that you are looking at a professional journal, and not a popular magazine.
* Length of the paper: it should be at least 8 pages, and at least some of your primary sources should be longer than that. Shorter papers lack details and often are summaries of posters or work-in-progress. 
* Length of bibliography of the paper and how many of cited papers are themselves published peer-review work. A paper that primarily cites popular articles, textbooks, and wikipedia is usually a bit suspicious in quality. 
* Quality of writing. If the paper is unclear, badly organized, and grammatically incorrect, it is difficult to understand even if it has correct innovative results. (But note that some grammatical issues could be due to authors not being native English speakers, and therefore may not a be a red flag for quality of results or discussion.) 

Of course, a paper may satisfy all of the above criteria, and still have incorrect results or a significant lack of details (which may not be obvious until you have put a lot of time into trying to read it). The opposite is also true: great results can be published in a high acceptance rate venue and have grammatical errors and mislabeled diagrams. However, as a first approximation these criteria allow you to discard problematic sources.  

### How to find supplementary sources 

### How to cite sources 

## Working with sources

