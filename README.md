Ballroom beat and bar annotations
===========

Description
------------
This data set includes `beat` and `bar` annotations of the ballroom dataset, introduced by Gouyon et al. [1]. It does not include the audio files. The audio files (698 files, size 1.5 gb) can be downloaded from:  
<http://mtg.upf.edu/ismir2004/contest/tempoContest/node5.html> (accessed latest Dec 2013).   
Md5sum of the file data1.tar.gz: 2872a3e52070bc342a4510a95e2fa0b8

Note: File `Albums-Latin_Jam-06` and `Albums-Latin_Jam-15` are identical.

[1] Evaluating rhythmic descriptors for musical genre classification  
F. Gouyon, S. Dixon, E. Pampalk, and G. Widmer. Proceedings of the AES 25th International Conference, London, UK, 2004.

Format
------------
The annotations consist of `.beats` files that contain the beat and bar annotations in the following format:  
`beat time in sec` `bar number`.`beat position within the bar`  
E.g., 9.430022675	9.3  
means the third beat of the ninth bar is located at 9.43 seconds.

Reference
------------
If you use these annotations please cite the following paper:    

Rhythmic Pattern Modeling for Beat and Downbeat Tracking in Musical Audio  
F. Krebs, S. Böck, and G. Widmer. Proceedings of the 14th International Society for Music Information Retrieval Conference (ISMIR), Curitiba, Brazil, 2013.  
   
Annotation strategy
------------
It is a well known problem that annotators disagree on the metrical level of a musical piece. In this dataset we relied on the tempo restrictions that are given by the dance style label of the ballroom dances. We therefore chose the metrical level of the beats according to the tempo ranges taken from:  
<http://www.ballroomdancers.com/Dances/>

Intros that do not contain any musical content have not been annotated, and should not be taken into account in the evaluation.

Whenever we find errors in the annotations (I am sure there are still some!), we will create a new tag in the git repo and commit the changes. So, please include the tags into the publications to assure the reproducability of your results. 

Contact
------------
For any questions or error reports, please contact Florian Krebs <florian.krebs@jku.at>.

Acknowledgements
------------
We would like to thank Simon Dixon who supplied us with his annotations of the first bar of each piece.
