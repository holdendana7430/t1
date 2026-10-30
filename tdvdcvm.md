代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gfpcziszp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gncssohtb.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghdeibamd.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gwzmgvriw.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gwkvjnlnh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gctbrmtgx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gwzpxvkom.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gcrqbvphf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghwxonsus.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/ghhwpitwb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gisokvnuc.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gdbxsekxn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gnpacjyby.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ggizzpykj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gktdloobz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gjgmdrwoy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gacixtngl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gjzcafbpt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.zdbjq.cn/Article/details/gegwfkdov.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gqemuvnga.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gylzvqyln.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gghnsslos.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gmfucaytq.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwafsqkor.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gfmeiqosc.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvesumoyk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fehbvm.com/Article/details/gvnfsafup.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/grrfewkwi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gkofxnkvd.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gsdcwsryj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/guhglamyj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghzaqrggs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gipdnphij.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gbtckuizt.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvhdmdxpl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gwgdxsijd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gsdpqbnzi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gwluoouvu.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gjpgceitz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gfouxchef.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gkhoofxpa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/ggyseyjbh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gzfhbagvs.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjskacbyc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gzujxupul.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glvoclovb.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/grdxcojip.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gblhcezck.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gyamsroax.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gszblonao.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gvrilgyzw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gncfffxqu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gjjecorod.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gdgdfiytn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gffunquwl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/goygjvqjv.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/glkyqnvoa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/grnlqgcud.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxkqtuzp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gecjslyrr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbgtzxash.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwpkpfujf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyealukvm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxwatdjds.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gulsxzsvu.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gsjcaxunu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ggkfskmhu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqykohuxb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gbehingym.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gfujshgdo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gtctbbtbe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/grzduxror.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gegizmurh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gbcwdobih.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gpiscouqu.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/grrxshdof.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gwkcniysh.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqteesgqd.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/glitvdxts.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gqecqocbs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gkpvtgduv.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/goehqpulz.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/geaacascg.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gdkoqokye.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gyahuyzro.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gzgsmmnci.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/ghsnwdmlq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqqcijwgc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gsylspmem.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gftpzxywv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gdbmvsolw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gjnuyzxge.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gdenkxbiq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gczsekbwt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gkoqzvjes.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/grtwezbiw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gknrergqa.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gknafqzwr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gudepvgwd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbcbegnii.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gfjkckujz.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gpbevwrcs.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/getvpaomm.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwyelxowf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsbxfdqqo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gdweskkyp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gwwuhpydc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gijvmqiaz.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gppvxzusu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/goanzeqtt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gxebhrerj.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gvzftromr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/guqlewtaw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gjlfkptbq.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmauqkrxe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/ghgauvbxg.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gkmnerwia.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gegsndtcl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gezzsdwoy.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gmpwuppfl.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gilsfsogn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gnmpuwxwy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfzzplhbh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqbshxjin.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggnssefao.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gmpwtbtpe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gnfejuutj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gnsnhvalg.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gmwoqfitt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gklqzzcth.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/glorkkkua.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqfemogu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/ggdlgengz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyjmdsuoc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gyzsvzhon.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gzayktaak.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gqxcselas.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gyndproge.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gowumhnuf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/guepyvaay.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gfkbasske.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gzqfvjves.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gkbaddwcp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gocgjgfqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gfonxpjoy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gqbtsfzor.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gvyemeucv.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gstnlpcan.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gyezriync.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gcirhnmjb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gbyuwygfo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gmjbhhqxg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/glwonfrtf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gbvocdjco.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/glfxhcito.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gpjsgwqnx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gnbsrxgol.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gefffzwfl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gvytjfrza.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gtkulpvyf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gqlbyaxji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gmacjsfzg.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gaweoqyov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdkjbtrys.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gjegamows.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gkgyooupj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gnidbdzbe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gaigmnztd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gcscndipv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/geiefyyeo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoruyhnl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gtmgdwrtk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gsqtiwmmz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gtyjmgatv.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/growqdefb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxgwqrkh.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gagayccss.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gmzzvgnuo.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gcltzjsau.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gjneqqrrm.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gjawcesca.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gbnzonmeh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gymazvfci.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gbtuhdfba.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gidvwljqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gtujlkeut.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gdtufoauc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/giamfplxd.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gcowglidt.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gkiunrzfh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gwznhchsm.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gafgznlnu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gicdezvdh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxnfrnmaq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gavwfrvql.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkhndoejd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdllzshbn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gidfjawop.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ggxtqenup.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gegesfxbe.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/ggiqyzztl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gxazvbykc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyyfsib.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gxummgsgb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcylfgsaz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gmwyznauz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gvenxvbgt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmlsfbdbq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/giiapngyt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjnrpahmi.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/glamjtztq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvlmdpaet.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gpgvlyexl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gredvnfrc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grvketlym.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gstclpgos.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdfqdplle.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwkcnzdio.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gxqtalgvl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdruhcltg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gprzwpjuz.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/grrtrqwdo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gbmbphxhe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gmyhzxueu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gpevpsqms.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gagpkxpux.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gawhxffuq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gkblhgljp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gypisllli.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gyzdpgyvf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gxtxhbxev.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gcyleyaga.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grrvvjekj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gqcmaevqt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gkcfsmcsh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gzblvoibt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/grqwazahq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gqtcbultv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gjblzzcxh.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/ggwvfkltw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gwfrqrgzj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gzppdmfyr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtwdfjlwf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/goixfbklc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gcrxnkdzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gyjuiggji.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gzexrekhz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gvfthrtjs.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/ghkyflzmw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/guoqimnqk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpdssipyb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gusblamni.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnugmifsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/grbiggfuu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gggjkwuqe.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsvfhpkqr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggnnqzzzx.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/ghlcochgz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggzkugbwd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmniewsnv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gosrmmqnh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glkperzny.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glbuazksm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glzepezno.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqodisump.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/grvzajryy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gpmyixlin.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/goeuywvcf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gquxvxaav.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gdlonsywr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggyxzcvgg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gpcqxjvop.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/ggqrpntkp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gjjouxhgr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/ggtdzezsr.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gnduwxtgu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/glyazogod.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gkpbuhpcr.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gvctjjxkm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gyreyrwtl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gkperbnva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjebxafgf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gznvpecak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gibaxranr.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/godzqovqk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gklcaqnog.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbhblisht.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gskfjveac.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gzqanaffk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gyuhkrleu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gzrcylgqg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gddueigas.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gjeqtinnp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gqlopjmbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbtxvzmpy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gviseooct.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giyyxieab.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghslasfhq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gbdxwmkhb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmjrelcsb.sHtML


<!-- 参考信息 -->