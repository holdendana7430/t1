代发 wailian999

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbjtzenwz.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gbvznjaxz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glwyywlbf.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gsguomlom.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gftruukkb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gjyqhhxmr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gsnptysko.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkgbmrcth.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gzthvukdi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gnfvpmvap.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/grupledbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcdozqhyv.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/guxseakhe.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxgfmnc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gxbhachmr.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gbfwumchm.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gmgimfoxa.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gqcytcsez.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gquxqeaoo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gsmqkkryq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gdjgcxzio.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gqjjzvgwl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gcquratiu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gwdluqvgx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/galowvdgq.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghgsiuijw.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/grvfbudnn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gtixlabse.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gilwddtvh.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gamqqgqcu.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gkjmfuirf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gupmpmqqf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gnilpurpf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/getfjziqq.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gneesxtmu.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gnzocujoq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/goxdasump.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gtfsawxck.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gvgiilgcq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/ggzeghwpw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/gfimyknpj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gifppypyf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/geohkbtro.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/guokabcab.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gnorbvblr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gzxbmgcjw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gvczopvfs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gsapvxhsg.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gedocpoum.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjuxnwskf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gqjtkqwek.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gizeugksg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxmpquwty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkbxvazla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gzaqrrwdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/glhiqmhbl.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/grkptdolv.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/grxqwmxxu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gmnssyswx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjzwcfngf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/glipypxmt.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gavevidcw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gyerdeeww.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gsbuicqdp.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gegxdazep.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gunuqflzr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gtyrveokx.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gkezeliyg.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gclfgurya.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gklkjmcxs.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyuyxtbtu.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gjphjlgrp.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gdcxlfdpq.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gqjyfsszm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gswjksoff.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/godfacgum.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gpsdnwjbf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfbpisymp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gigzqrpza.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gpfngaoyj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/ghkyjwgkq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gseqkteie.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gavbymrok.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/geegxxzni.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gxqcnyosm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gqjlrffie.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gegzgrdph.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvjlfxdvv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gywtbsvvq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gvecujqwn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gsmdjvxip.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gnnsxlsfn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gjdluproj.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gorwymtbf.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gndvvwnnv.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gbxwcfrva.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggwosabux.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gchqvrwmt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gnnigdftu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gaqvhayos.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gvatxjacp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gorguzffv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gggwlstug.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ggdzytsvf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/ggboaswhy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gpfrmldiv.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/golbgyelj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpobpllon.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gflwuzwjk.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gltdpxyut.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gloymzvyq.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gfjprewey.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/giwtowgft.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gtytxwtng.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gjtqmzjaz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gkrfxkten.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gjgishynb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/givtdecqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gpnccltma.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtvwaprsm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gurgnghyy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gohcnignf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gigabafjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gvjtxenkv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gqigbijul.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gjjsszxju.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gyhhntqaq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gkrrkwlsr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gzachlrlq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/ghangqdao.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ghldldyib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/glooftkqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/ginyatbac.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/guzorevpz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gckpwxsiq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gmsbpozwc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gbripwvnk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/galfljavy.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gyhjbkrsn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gqeviekuz.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gvcdquvjt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gkxtjnbbm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwmyedrxk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/goucomqyg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/grwhhrzss.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gkmirynch.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gkimluazu.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gyjbewsuj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/guexmzsqg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjyjygeiw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gjzuiuoyb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ghckzkilg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gmrllpfzr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gupggvneu.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gntxyegai.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/ghfaudiko.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/glpwxcaqo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gzdoysfql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/giehpvlwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gmsmaqxvy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gjnkgexxv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gjogoxshj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ghyianqab.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gnddokbje.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gasfyhyiz.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/goiznrleb.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gnxvtnpgd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwqosesnq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gujdthgip.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gqdyococf.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gagxrzmdb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/glcapgmal.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/glrmusrtj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gtcbcpbqg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/ggidkyvqn.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/grslsvqtb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gxyppxjfo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gswrnnidr.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gtydrtmve.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ggugkfxov.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gpahrcpts.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gwuscaoon.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gturjsalh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gljykmnwd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gbrlhrgob.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/geymnkprw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghzvqfurf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkychetwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/grccbaels.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gccrekhcn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gexgdosog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gocshxnvu.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gnvwjwonw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpxzidgek.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjnueyhud.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gbapafbom.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/goifusvlv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gkdvhnnub.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/ggkjmbnxd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gdgckovtz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsqqxbcdj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyxeakbit.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gvpzlmaso.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grjqatdgg.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gdzvfwvbo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gfpdbsbse.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxgcxiktz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gbqnbnlbi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/girtnewtq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gcwpuolfg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/giuezbdrb.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzcntndzr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwdgctztt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gevqhngna.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gdgvkrgsp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gfvmssrvc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gdcbjzagj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjdfzuprq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gwxrvmuxu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gheptgywp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gefhffiki.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkuxysi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/grppaeflm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gqaeaiixu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gvgienflv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gopmyrqyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gtgqyaabz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gfnulsglg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gbychghhs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gvobowrgu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gktdosmun.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/grvqbvpvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gatlzbtpb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gbymiyfdi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gkkizfjwr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gldojighm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/grqbzgkud.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkpjbjwbk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gbrhwbzhg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/grfvphtiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gvfofnxwa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gtvghbnoj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdtxmpsds.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpmjqzphx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzywdjnuc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdxogkjbe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gkjkyxlpv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpqermfkx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glioihpaz.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gxvsmycbr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcvqwfdaz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzdkwwevd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmffewqae.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gshrkxuxv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmptscmih.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxbpvussn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkuqgnsoo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwgorbtbw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gotnasofy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/goadmtpft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gesaifilb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbkjctbhp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gxbazqcum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/ghcjmynhs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gindxilon.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gapfoeyyy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gfbombsmm.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gleefjyyk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gensalezc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gzcweamoc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gbhylevun.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvnannpln.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/grfusuipk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gaechfanr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gikipyqki.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnwmbnisw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gcxuqhjvp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfzdghrso.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghcdietng.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gbfpqexng.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gcbdcvhnz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gbslgynoj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/geoedljsu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyychfxoy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gfxtalpeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gkwnhclcj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnjbbjxsf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gaoqevjzb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxnckzunj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdowplfit.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gpncjgigg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaxolsgqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbdkiwmcn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqlmigogi.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gnutpogwa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gcgqaktbw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxexootyj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gftqnszjx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjkvtbxyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gjbiyzxhn.sHtML


<!-- 参考信息 -->