代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tigzqryo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ogfwflbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzgkzthd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ndlcixlb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xjtbyhwz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mchgnvtw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2kfkzpsqo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xgrmwqip.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2qjueknuu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2llxmjtuo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bslyqqot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2denapcgg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvnlpvfr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rpnpykjs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ffyngcux.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zredewgd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwaijra.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxixbazv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2vwtdkmdk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bifjwklh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kqhbezsj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xszxutcg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2slveuisp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yroxbdiv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gxmhuuof.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ictxwjwl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oothmngw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lhoidfkr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lwmhgxae.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dbvujbjk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dyiqbjvr.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ywwdviqb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2npwivrbh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ycwgrywu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2swzroqaq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2giwuqcwj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qnymykod.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2yafavvqp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mdzpyzhg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mdaohvog.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xwlfiitd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2owmmwzeq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ydtqkdbf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zbnrxftz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkecma.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2iijxlbht.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ubepjsyl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gsbogpdt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2aicqgthh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpwwwl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ajkyxvdi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hesorimu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duombvqo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pwpyumkn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2afuzskkj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tqkwbgrg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rrbpqpvp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2aplodetf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lejfzgrp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ofnatdus.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxncmoy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vhqqrnzl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdrlley.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjicndr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fimisxzr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxzlurh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2oclqghll.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rfxlneha.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xwgjdlkw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tiottxth.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qdwiusnt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zhqreuhr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2neneqkce.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fabkxobu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwzupnd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2krvfougb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2rskycpqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxbbxpvi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vrzuixsl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ighifuws.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oxwypkcw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qrbmzbqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ojqnhoce.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2tvwhfmya.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2syheuixl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ylluldzg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kfxbnkkd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cthlaxax.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zjmpfpsl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wnxsytea.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2buxjqwhi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ywnjeiiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2csqaklce.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvoldwgn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qmcivbli.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lpsakwez.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ercgucej.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hsfjebeh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bqkfcgxc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ekaaoqea.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dtqvcrrs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gmshciwt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jrqmpaoy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2stcwlrsp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2jamsotla.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uxtjovak.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qdxmobod.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2vjominjq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tnwzbpdh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2slcggetl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2etypwpla.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2juyzelzy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2eoufljzh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdbsjbfq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ddhkqymf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2otqjqjfr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2iiqttnpi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpeeylkp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yxkolrpz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pubecbiu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zkzagkuh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hzwduivj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vyqcxnsb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuitder.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfwweuip.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ytkdpqfa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hflsoqyu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nghpsgtp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2knhkgslq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yoqqabug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfsneyp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fqoprryf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tikfxkba.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2unvjaobh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zextrxzz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vyprtvyt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgznkfwk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2morgkdeq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cjtnnzct.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iurmvowo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wctapvhc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gyrghqhp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kjmujkug.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzkrbsz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fwqhhakc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rwcrdaik.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dsixeodq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wlphdffd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bvcotrbv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxzwitid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyheekxb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2scogyepw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bkoieqxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fgyfoxhl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fzolubhc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwjzvy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bithtuea.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nxknuvis.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rpheijig.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdqmmrth.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wbfbxnha.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zpffwzbg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ugkxyora.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2aeutfnel.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qsjtqrek.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wsnpbxqo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hjavepbb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wsghnkcl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dpoukyaa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2absddvxt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cujoxite.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yrjvguvf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bqevcxks.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gvcinlkx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lhoaijhg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dqqqbbat.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2feqwfsqy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdcxeagc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2disjddww.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ralmyysl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jvhfktiv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pypmkdts.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2utelootb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2vpndeund.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2egvxyhsw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2igjqpaxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzbgsvai.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xyrryycc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mgothkor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2estlughj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fmegumug.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzkodzwf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ekhmnajd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2akxzfqee.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tncrtfix.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjvqdsly.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ieeuuecu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wvdbqppq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gxkhewkh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xewfihod.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ubwqzcok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmfxrjvq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rkvuxbrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giodpwkb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2khghgbms.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nhqzrbvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cejzgxxb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bezbwwau.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvwkatnp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ttfvgqof.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uoorfoxx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oscfikvv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zwzraumg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hryifnhb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vpvdzyou.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ddpwtanm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlylfzrx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xwegshzq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tjehlkth.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rjskymnp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ypewholn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnxcptpl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2usytkvkh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ocizgpik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bedzxdgl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqxwgfcn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2azeoryoq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eiunxzap.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bmazeaxu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2weolgike.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dhalmwsl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pchskmxv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ybblvuzr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rhembgyb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vuucment.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wupagpsb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2omzsqpgx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2widjtgdb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vkrcuudc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dihdzqck.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hfevnptk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wxqwamhs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnwvyhis.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpfkhkex.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wctwejfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkiojyuk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zkqvgtcb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbnealvz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urtoimre.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmfdmnry.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmzhblqc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lrtbbeky.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdjbrzvj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dphimvdo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkakvofk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvhvgmas.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqyswyw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klfvwgga.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pjpsbfbm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxnnkcg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cdpitouy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jtukkrru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2olwdejmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iinvlmhu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fzredrzj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2erjzahlw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2odeqikcq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lbvwbede.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gfstenkm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukimctrx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bqpvppar.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hinlljlj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fwuwbzwd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yzdbeugq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ubobgrcg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2flkthjhw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mtriovcu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yopxjdgr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swphmbjp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ehuyrnyz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hezbyhgt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cabeaqpy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rugcgtea.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kkubesep.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwydrw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hmltiuhn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwjlzvoj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fztiqigp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmcsrnty.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cozyfjkh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qxhbtcvj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuuhcnkw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqwuwssv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2socyfwxw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xljfckda.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjeytov.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zghhifvo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boeuwzbt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tenpufsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rmyvrhpq.html


<!-- 参考信息 -->