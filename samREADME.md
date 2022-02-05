import pandas as pd
data={&#39;name&#39;:[&quot; Abhi &quot;,&quot; Bhavya &quot;,&quot; Charan &quot;],
&#39;branch&#39;:[&#39;cse&#39;,&#39;cst&#39;,&#39;csb&#39;],
&#39;age&#39;:[23,22,21],
&#39;marks1&#39;:[500,600,700],
&#39;marks2&#39;:[550,600,600],
&#39;total&#39;:[2000,3000,4000]}
df=pd.DataFrame(data)
print(df.aggregate({&quot;age&quot;:[&#39;sum&#39;, &#39;min&#39;]}))
df.aggregate({&quot;total&quot;:[&#39;sum&#39;, &#39;min&#39;], &quot;age&quot;:[&#39;max&#39;, &#39;min&#39;],&quot;marks1&quot;:[&#39;min&#39;, &#39;sum&#39;],
&quot;marks2&quot;:[&#39;sum&#39;],&quot;name&quot;:[&#39;sum&#39;, &#39;min&#39;]})
