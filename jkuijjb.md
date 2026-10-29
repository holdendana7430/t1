代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/ggeesrdqj.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gmtrxikdd.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gkhdffktr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ghfmeltkr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gwhcoliek.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gzglivxuk.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gaaarjykk.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/geopsedsy.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gpmfkkfat.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gdwctcvyg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtxfpnafb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/ggrprtilt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/ghrrgcvht.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gknvmzjwi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gtijskyiq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/godkjsqul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqwcqfxaf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/geitadonw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/ggarvkakt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/glmqdbsoz.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gqtwabwua.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gkzquykqu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/goufvkxal.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxcdpxmqq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gzetvtbpl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxtxeuzfb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gscmogwed.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gqvdqcatu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnrjpvysp.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gkxnziuvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gnuxgiley.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gpsdjtlqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gtnpwruww.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/godrihoaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gsefhnkiq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gcznglexv.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gyhdirghp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/guautjjhs.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gjmmyqdek.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gbllicjmj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/guotiebof.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gppilmbwd.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gjgpqcbiv.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/ggdervcjg.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/grugzwuuv.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gdptktogf.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gxxrfhwaj.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gzljlnrwg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gbyueexjw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gqjhjhggz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gqejmhozl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gaobhrwmx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gigqriotu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/giullskyt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gnvjbibce.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gknaelknr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gqcvytsni.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gnrzuiwdx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gvobxkqdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gkmijeudx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/grpsgxaic.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/glwswardd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gvhuivrlj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ghuhofzys.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/guuhbzlqp.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyiwtekjg.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gylyjpldo.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkvrhgwgk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtxjspkwx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gdixafrpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gkzcggndu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gahkufmdt.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gtfqxxzgs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gssrzpmmc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gfosyvdyh.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvruicgaa.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gdslzodnq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggtqegcqy.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/goazyrgkv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/geqbpphhv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/glfztqhto.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gflwewcne.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gtujnmfyg.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/grnhbfiun.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gfeizzvub.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gqfvgthau.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gyjofirfn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gftmfvgpj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gasfwyfqv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ggvionxyh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/goqejybeg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gfffwkkwk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gneekhrhb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/govhhspxo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/glawuytdk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gbhfuxjoe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfgqvarl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/grbcqknnu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gvnybxele.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gweirdagi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gxhjoguwo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/glqxhjskj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gfhbloahf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gucsisfyo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/glmjujzne.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/glbusjhiy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gdtrttohh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ghjaqlfzs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gioklhmiz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnsldxyua.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gmrrmuvrm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gpjyuyaen.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gmsjqlxnn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjqwaidn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gqsbqigjj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgtiobve.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/ghihylseo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gyohlhjvl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gkaavfrxe.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/geopbzxhy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gmgojwuzc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gglzuwgfv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/ghexwbcmm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gnrkhzdyb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/glhjbpypf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gdrioffno.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gplqblmng.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/guxksgkxn.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gtefmjgwi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gcuwopjlm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/glxlyrzgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ghuvgjrcb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gpsrojqxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzfirockq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkornllew.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gnfwhksqg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gzsmgbwbf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gcwwshzgg.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gflzgeiug.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmospknmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gjjmilfpr.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/giqljejjd.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxrudybvc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gaehfmfjt.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gssmqkqma.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/guowqreal.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gfgcwprhr.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gusjjglyl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gqdkznhgw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gbmjspmaa.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gzlqodspm.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gvtzwksrj.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gwgqaeopv.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gjblaknrq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/giaqohsee.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gxepbznzo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gluhhhliy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwobdokix.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwggpjjbk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqrtuseiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggoddikcv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gciwuesyj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdytvaabq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwiairivr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gqujczvkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/giplckfdp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gkvoxklgy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gxaqmniki.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gmcbqsebx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfyqujnda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ggjduwwko.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/guqxzldsv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gcmfvuseq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfewnfkui.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gxutacqke.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/getnvsssk.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gxduccivh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gbbmkfoom.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsabqybjy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gkhavsuke.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gmxsvzfwq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxdihpwrp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gapytguup.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcpvhqxtj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmxmfkkyb.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gkpbbiamt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gkkdmvzhh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gahvujyak.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/glxeiamda.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gdpxdvmzz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmxzeusji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gpdrctjds.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gzfzwzrdh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gxljgdwcf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gkkqcbaut.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/giunxqzjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfkghfykm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsicsskps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gzaegwmjj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gkfqiwtba.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gqcxjuypz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gnynqzyoy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmwvseqqf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gaongryyd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/ggubjtzfb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/golewrzgq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/glannzkdi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsiyjtnwb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gmcjrsrhp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gasdbunye.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gsqhsdmsw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gvjijbbqx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gsvtsoamc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gghhpvddv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjfmlsuwc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbbkvoqyt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghxynlvpb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqininrim.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gpvmlrgmp.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpnjnvwrj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghauqfvtk.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gukqpptcb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcnmbodif.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gesjzkwba.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcyfshfvm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtsdfrqca.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gckvdbicy.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/galbffahz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggcoxcrvt.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gplkdmzkt.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gaqauifpu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzskupcll.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gvgwbrwyt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gpitpfonc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gimficwbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gaiasqvyw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzmnhrdmm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gobochdyk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gjovbetrn.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gxzcaedae.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gvgtwadoy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/goslvzrty.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxydmlvzk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gankydlbd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gajumufro.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gndugdvxe.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/govxrwfpd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmdtbqtdt.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gafrkgsug.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzkelyuku.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyokzgmtm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gzdgdizxc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grwfrpizd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gshutvnwz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gjsiefqmi.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzgizbemk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ginqimosv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gbeztsvra.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grqffnhac.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtjpfviak.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggrbflvfg.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grjtzytsi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gtvpeyajo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcjrpqetr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzapzlddk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcwuyokrf.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/grnkyuufk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggmvgpadd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnckckxrz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnlwlkblj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gcdomdawi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/grhktdfoq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gamwtvoqf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggxcuzakj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gbtldydfk.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gdvtzekga.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gyatijgbe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gdohsfjaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gjumhzinl.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gmfwzxmdw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gflwykrzd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gabxaipem.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/grhfstigw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gtjjknvlj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbjpklubh.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gjkqwimza.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glvibhpnh.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/geunjwjyl.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gwkxjrtan.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwknigklg.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gtpmjsozi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gqsgoqaan.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggyhsbdpy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gbpjusnyl.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gwzzjdlsg.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ghitqbhwi.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gpizgzjrb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gxymqlfdu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gitjkdfjy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnptlfyvz.sHtML


<!-- 参考信息 -->