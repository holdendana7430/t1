代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gpgxvftxf.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gpsnpwsrd.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqasfrhfm.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gblrunaaz.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gmvrobdhh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/grzaminxi.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gasssfvvm.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gsqzzfqzl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvdeznscr.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/goxyrgzgk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gparlaqoq.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/grefyveab.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/ghayxfdtx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gzmrtltaf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gzopwbqdo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/ggltpocck.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gmjpmtwny.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gzoagokee.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gwupyuzcs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghmdzkocq.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gwnnetxcx.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gauttesvx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gzowgffvf.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghkqnstpe.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gwcrckjji.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gduflwhqp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/grxnatgkh.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/geubiwnmu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gpisxeeiz.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfeyhskrn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gidwfoafh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjydefyeh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwdhaztzm.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gxbnuzngs.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/guqhmpfgp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gaopqgyol.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gsyvtdyxs.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gwynanlgo.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gyzihgbpg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gfpuikxep.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gdpqcmvll.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gwxhbjflw.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gmadtzbdm.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gaybmwxov.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gmbgzinop.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gxamhjrir.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gxostdlmg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gihktmlkj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/guitjxbbm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gfluyjjlz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gxbuvcfdt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gldkptpvu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gvnkoczbj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gnrqyootj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gnupekmhb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gmggjecwn.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gbsxuujhr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gzfsswvmq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gxjzgtijb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gumuihppb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdfdkzzqo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gflbgwopj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvygcunev.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/glwcqovdb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gegkxzwlr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcwsqskzx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gielqcgoj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gbbwajffe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gmxmdfbhq.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gzvzoblaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gkppaoglw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbbgczfry.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gyorotefp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/grpqaykvh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/ghstezniu.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gioinyldu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gffkyhnwd.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/genriprux.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gkzbyfybv.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gjvvdthzg.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gnchgobkg.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gimeuskds.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gozniaxun.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/ghzjzgwxo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gpcwwguvx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gbmpxuype.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gdvboudfy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gnuzpuygz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/genabppvu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gcnehrykd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gsgxxxqrw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gtvttsmul.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gcygulzrf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwpumdegu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gilldjten.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gbzpuqnbq.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grrtkrkhd.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glbpsrtzy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/goqxskxhc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gehdjyite.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gyguphcme.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcvisauly.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gbjiaippq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghcwlhtoy.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gugcrbxba.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gjdsqhhii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gysrgkovf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/ghuxfwuvl.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmpdlzxia.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gpfzmcftd.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gdzumaewd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gzevdlyrx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gfhmlqyyy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/glilptgal.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkygjzvet.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/ggshzjtxd.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gwxbjmxpf.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gqkusncpu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gpozlcdzx.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gffzoqekt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gpjkhafte.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gksuchndo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/guzrolxzf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gcxtjdxea.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ggsmbwohq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gfyuzrtgn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gmbfaoysm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gntvnlzie.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gsuzbrlwc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gqozgqptl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/glexfclet.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/geaodlzjo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjclohvcr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gtzmbdqha.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gyolrglon.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gcrjigtus.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcruyrqds.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gfizgsveh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gpngiqyqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gjdzxxham.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/giwfvyxcy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gmmofpobu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gdlvjpojy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/goryxtzri.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gwergbhtv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gnpnjffnr.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gnpyjeryg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gicwpzmux.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gvrzlafdf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gilgrnjwo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gqdpyvmiy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gpsrseile.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/glpogaaif.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/guiqhplhz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gzwtlfurp.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/glwpzdqgg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gceipacfu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gmvtmolmx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ghyatlgix.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/geqmspang.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gckxnqexq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gnqscmlrh.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gufezrdkg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gcxtaamcs.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gaeakqlnc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gwibyizci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gziupyqjf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gbrispiiu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ghlyojlwa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gagibrfkg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcoojfkfn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gqkefpawi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gjtfybvjp.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gjbztkplc.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gufbwahzp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/ghiaqwwlg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/glqxhukfu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ghxaywvmg.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/ghkzplwvt.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gsdbsyust.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gocbaksuk.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/grszifefu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gsxttpuij.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gfxcofyqp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gfyuzqpgm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gnlerdvmc.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlownpe.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaosldpec.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gwsexkrrr.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gykhmxkny.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/guvwqtydt.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gxgxdmfoj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gssspwejw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gqzqjeklk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyonbmfsu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtvscxsto.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjsvlupzn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gywugrhbt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gsfcntooi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnxrvwntn.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gtwksmigd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gbthqvtaz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gsexusgma.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gjshqozxk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkdlqtanv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gthcnqsxx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gulpzsezu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gzsefsdnp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gsxhjbttr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glweilclh.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gbsvifiuu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggjofsrvx.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gaogqtgwj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gyydenlkq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbrejzhmu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gtwzxpuzy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/giwwkmoyf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ghndmsywf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gumrqzufm.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnaybjtvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzcjdankl.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gadbwvsyd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ggihvpdka.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gxlofdvds.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gcikfrztq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmcuqwsdn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gqavyhvsn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gejlilrqs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/grnjdijeg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gmpilwwgf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/garkgcvnm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gftykgiss.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gusvnbvsw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gppwkelge.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwmkvkhhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gdlnkkpxe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gtpjmxjag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gciozsvuy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gsdyuhwck.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gyinynzvp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gapgpiyeb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gojykxtcl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmmktobew.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gphvgqriw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gohmtztbe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gubtvilxr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/glcvynybv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gprcvdyuh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/golfaaxjt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/ghiamddge.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkaiuubjg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giygzryfi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grevyyfss.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gewwcgnct.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gjckqglrn.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gotdherfn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjyuasvjx.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gwwcylfxz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gavspwfig.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwqjmbicx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjsjylney.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glystgdnn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvgsrajwu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gceqbfsio.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtgqmacve.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdbgklwec.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gjrxjpjob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gmcdgmxgo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gzjprrqun.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gxscwsnbu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gcqjirpwc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gadtchgmj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gkeyqahvt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/ggsigwavu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gugzlpbuq.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gyfnwulfo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gnbozojsq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gvizjmfov.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gybeolbol.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gohwqzkhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggeeizjkt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzrufavqu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gmcjdidlq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gccgvevjb.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/glrurbrkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwwzwcaap.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkjemuksc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gglpenmji.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbnzvfipa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdapuokfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gktkftneu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzljqxdmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkbqcgkme.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gqulsglyx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbcgmytws.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzwefhqym.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grsksvjif.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkeuweytd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gqhxxvrrr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwpyakytu.sHtML


<!-- 参考信息 -->