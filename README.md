java c
STATS 3DA3 
Homework Assignment 1
Instruction 
• Due before 10:00 PM on Friday, January 24, 2024. 
• Submit a copy of PDF with your solution to Avenue to Learn. You   don’t   need   to   write   the   questions   in   your   answers.
• Late Penalty for Assignments:   A   15% penalty will be applied for each   day   an   assignment   is   submitted   after   72   hours   past   the   due   date   (rounded   up).    This   includes   accommodations for   extended   time   through   SAS.
• Assignments submitted after 72 hours will receive a grade of zero. 
•      Your   assignment   must   conform   to   the   Assignment   Standards   listed   below.
Assignment Standards 
•      Write your name and student number on   the   title   page.      We   will   not   grade   assignments   without   the   title   page.
•    Quarto   Jupyter   Notebook   is   strongly   recommended.
•    Eleven-point   font      (times   or   similar)   must   be   used   with      1.5   line   spacing   and   margins   of   at least   1~inch   all   around.
•      Use newpage to   write   solution   for   each   question   (Question   1,   2,   3).
•    No   screenshots   are   accepted   for   any   reason.
•      The   writing   and   referencing   should   be   appropriate   to   the   undergradaute   level.
•      You may discuss homework problems with other students, but you have to prepare the written   assignments   yourself. 
•      Various   tools,   including   publicly   available   internet   tools,   may   be   used   by   the   instructor   to   check   the   originality   of submitted   work. 
•    Assignment   policy   on   the   use   of generative   AI
–    Generative AI is not permitted in   the   assignments,   except   for   the   use   of GitHub Copilot as   an   assistant   for   coding.
– Clearly   indicate   in   the   code   comments   where GitHub Copilot was   used   as   a   coding assistant.
– In alignment with McMaster academic integrity   policy,   it   “shall   be   an   offence   knowingly   to   submit   academic   work   for   assessment   that   was   purchased   or   acquired   from   another   source”.       This   includes   work   created   by   generative   AI   tools.    Also   state   in   the   policy   is   the   following,   “Contract   Cheating   is   the   act   of”outsourcing   of   student   work   to   third      parties” with or without payment.”   Using Generative AI tools is a form. of contract cheat-   ing. Charges   of academic   dishonesty   will   be   brought   forward   to   the   Office   of Academic      Integrity.
Question 1 
Open the   surface weather   dataset   at noaa-gsod.csv (a   subset   of a   much   larger   dataset).    The   larger
dataset   is   available   at https://www.kaggle.com/noaa/gsod.
(a)    Read   the   documentation   on   this   dataset.   What   are   visib   and   fog   variables?
Hint:
1.    Visit   the   website https://www.kaggle.com/noaa/gsod.
2.      Read   about   the   variables.
3.    Then,   find   out   what   are   visib   and   fog.
(b)      What   are   the   data   types   of   visib   and   fog?    Use   the   data   dictionary   and   the   data   type   in   function.
Hint:
1.    Now   read   the   dataset   at noaa-gsod.csv.   Let’s   call   the   data   frame   df.
2.    Find   the   data   type   of   visib   and   fog   variables.
(c)    Use appropritate visual tools to explore the distribution of visib   and fog   variables, seperately.   Choose   an   appropriate   scale   for   the   vertical   axis   and   colors.   What   do   you   notice?
Hint:
1.    Find      the      type      of   visual      tool      for      each      variable.       You    may    need    to    covert      the      variables      to   appropriate   types.
2.      Write   down   what   do   you   notice   from   these   plots   (missingness,   outliers,   any   other   patterns?).
(d)    If there   are   any,   replace   all   missing   values   in   the   visib   and   fog   variables   with   explicit   NaN   missing   values.      Comment   on   how   do   you   identify   missing   values.
Hint:
Missing   values   may   be   an   unsual   value   for   the   variable.
(e)    Create   the   visual   tools   in    (b)   for   the   visib   and   fog   variables   again,   ignoring   any   missing   values.   Provide   a   clear   and   concise   description   of the   plot - this   description   should   be   cast   in   the   context   of the   surface   weather   dataset.
Hi代 写STATS 3DA3 Homework Assignment 1Matlab
代做程序编程语言nt:
Describe   the   range   of   values.    Describe   the   shape    (bell   shape   or   right-skewed   or   left-skewed).    De-   scribe   the   mode    (peak   of   the   histogram).       Description   of   the   plots   should   be   written   using   the description   of the   variable   found   in   part   (a).
Question 2 We will use Spotify   Tracks   DB   dataset from   Kaggle,   curated   using   the   Spotify   Web   API.   This   API   provides   detailed   information   about   each   track,   using   the   Spotify   URI   and   Spotify   ID   as   unique   identifiers.   Download   the   SpotifyFeatures.csv   file   from   the   provided   link.
(a)    How   many   observations   and   variables   are   in   the   dataset?
Hint:
1.    Go   to   the   link Spotify   Tracks   DB   dataset   from   Kaggle.
2.    On   this   page,   there   is   a Download option   at   the   top   right-hand   side.      Click   it.
3.    A   zip   file   will   be   downloaded.   Then,   unzip   it.
4.    Move   that   dataset   SpotifyFeatures.csv   to   where   you   have   our   assignment   notebook.
5.    Use   pd.read_csv()   to   read   the   data.    Let’s   call   it   spotify.
6.    Use   appropritate   function   to   find   the   dimension   of   the   spotify   dataset.
(b)    Verify that track__id   is   unique   for   each observation.    Comment on   your   findings.    If duplicates   are   present,   how   many   duplicate   track id   entries   exist?    Remove   the   duplicate   tracks   from   the   dataset   before   proceeding   with   further   analysis.
Note:   Duplicates   may   occur   because   a   track   can   belong   to   multiple   genres.
Hint:
•    Use   is.unique   to   check   duplicated   track_id.
• Use   duplicated   and   sum()   to   find   the   number   of   duplicated   track_id.
•    Use drop_duplicates()   to   drop   the   duplicate   track_id.
(c)    For      each    track_id,       there       is      genre,      artist_name,      track_name,      popularity,      and      some   features          of             the          track             acousticness,                danceability,             duration in milliseconds,   energy,          instrumentalness,          key,          liveliness,          loudness,          mode,speechiness,          tempo,   time_signature and    valence.          Analyze      and      comment      on      the      types      of      these      variables,   grouping   variables   of the   same   type   together   in   your   discussion.
Hint:
Use      .dtypes()   to find the   data types.    Then,   comment on the   data   types   for   the   above   variables.
(d)      How   many   unique   genres   are   there   in   the   dataset?
Hint:
Use   .nunique()   to   determine   this,   along   with   other   techniques.    Note:    There   may   be   variations   in   genre   names   due   to   ambiguous   characters   or   formatting   differences.
(e)    Calculate   the   average   popularity   for   each   genre   and   identify   the   five   most   popular   genres.   Select   all   tracks   associated   with   these   top   five   genres   and   use   this   subset   of tracks   to   answer      questions   (f)   through   (h).
(f)      Visualize   the   distribution   of   genre   using   an   appropriate   method   and   interpret   the   plot.    Ar-   range   the   genres   in   ascending   order   of frequency   in   the   visualization.
Hint:
1.    What   is   the   data   type   of   genre?
2.    Choose   the   appropriate   visualization   method.
3.      Interpret   the   plot.   For   example,   which   genre   mostly   appears   in   the   dataset?
(g)      Examine   the   relationship   between   genre   and   popularity   using   an   appropriate   visualization   method.    Ensure   the   plot   accounts   for   the   varying   number   of   tracks   across   different   genres,   and   interpret   the   results.
Hint:
•      Use   the   width   of the   boxplot   proportional   to   relative   frequency   of each   genre.
– compute   the   number   of   tracks   in   each   genre   using      .value_count().
– relative   frequency   =   counts/len(dataframe)
(h)    Explore the relationship between   acousticness   and popularity.   Use   an   appropriate   visual-   ization method to avoid overplotting   for   this   large   dataset.    Interpret the   association   between      acousticness   and   popularity.




         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
