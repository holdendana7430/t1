代发 wailian999

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gojgvkdrz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnjiyhzdx.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gqfotvjqb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gmjxvtnkz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyzllrysa.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gskbiljoi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjkxiqzst.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gdakglybs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/ggtuivaiz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/ghqajyzmg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gvavbfwlm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gkupspdhr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gmljqzvpv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gozzbrjvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gvgrvhyvk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gyfbbllxo.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gonuxamlr.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/guhpnazwv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/ghsyhbhjn.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/grtstrlch.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gwdwkbazx.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gjovyuxtl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/gdbqsmkje.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gkciufals.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gxilcwhvc.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/giutnaswz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gtuzhiiga.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gniyioukx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gcwmocvir.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gmlihmsnm.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gmhuqxstp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/grrcxbbcl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gayauotzb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gcadxfnig.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/glhqkjdyf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/ghspgstko.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gkjfxntso.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gyqnhbtpl.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gefelbhhr.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjiqbobjv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gjprinngi.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gqcwrkkao.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gvoochlpu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gpszvmgqq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxbzuhvwu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gtyuqzdlf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gswqzixkf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gibddjgni.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/ggbxxksnf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/ghvwnvulc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gqcbzjsip.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/golwwnnsl.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gzcmkgsqb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gnwxamzfu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gyddtrwdg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/guegfzcul.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grvrskvvt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdrcxupun.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gaiinihbc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gvhmbatxk.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gyzlgfyod.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/giauaxaen.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gslswkytp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpuvrxtqq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gbpohmceo.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/ghjbrsmll.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gobuvbowu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giepgxkqy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gavuolcnn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gxpoiotzn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gumodtruy.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gjlvdworu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/glnzasprm.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/grcciwnte.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/giwjfnywq.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gycnszkvn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyawvrvff.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gokawjxjs.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gcxngyctz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gvtmxqfpy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gmtzfurpa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gkuglzvai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gwfjzrlyt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gewuhpfaa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gswbanzng.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gttcmtkkf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/grfokueut.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gaojoyyri.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gphumtlea.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnctbnoom.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gtgsqsnip.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gwpdsjzgu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/glqlwimqy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/givxyuzul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ggewwzape.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gdsxzrwge.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gpjuqjlvr.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gpllwhomo.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gjgrjtlxg.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gaghhllso.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gezkvfjdk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gkppwuhxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gjranamlm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gmndjiihl.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gjecrspqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gwomhxxqu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/glumpdysm.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gimtphqgc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/grrxugtia.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gnsagcstv.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gcfhwwvgd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/goeavaiwk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/glvzuccup.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gkkjmbjav.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gjuiypaqr.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/ggimcnuii.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gvvbyzowx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gqdyqqbcr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/glooolhdc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gourpbkyt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxincjjka.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gwfykjowa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ganxezmqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gobyagxhx.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gbhducirl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gaslpyrva.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/grkpdnhkk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/ghbkepzbg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gtcannixt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfvsmtfcv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gistipbwm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gbcqzanov.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gajfwoeln.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gdwkrmxch.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gsaqnbyeu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/giuuzdocv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gehokysly.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/guxwjeuhv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/guxgqciav.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gmynsuelq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guotvvpic.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gawpulftd.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gotihkxij.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbxmozfai.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gjgklbrqf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gihlaespd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gdlwjdreo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gpaufxguy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gbbshkxyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gbzuudcoz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gpwcajdhs.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/guodirkro.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gwspnnnbw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ghkjlnyys.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gysbbfxcv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gtcssbbxy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gmtchutzd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gifpcbxhd.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gcepdjzrb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gasdysivx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gqiqewzxm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gvcjzqnub.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gsyurjaww.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gztnxnozr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggptcdxxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/grlxktcgk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gorimhcln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gihdlkapi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gmulbapjd.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gdzlofjcp.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/ggindojbm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvtykozlv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gspdemwfo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkidikjq.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/ghgtnpfge.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gzwdgdyfn.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gzxqpikcj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gnngjoelh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gauadhovh.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/ghfwupvgp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gzdohgmsb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/grfvpqbls.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/goksjgvvc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/giwokjzsf.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gcffjhotd.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gddovaqla.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gbvyunlrm.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gmmfvhdng.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gfjgibnsg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gfmkwdbrh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxzzvjykg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzpawlaiu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gzdqrivxe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/guhdzkffw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnsmxqsyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ghmxkdhue.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gllitswoq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghydwngwm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjblwlinx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwecjluun.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gmywxlnep.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/glrdrisin.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gpfghpshx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gblumulku.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gfzoajpxl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghjpnuewk.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gmdwywgqs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjbpaoywk.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/geitdmpho.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gqhsyxndm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmfojxmxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gxbdtqkfg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gldalvjzn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyqycbykg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gwemupbxj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxnqfyvzy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqjidguuw.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gdysiqnle.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/glvtnziap.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gkkikpsqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzujicelk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gxixbfone.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gvdxwwcbj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gjtdivdgl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/glzpxqies.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gmsddeumy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gmnemmofy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gypzttmva.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gchiqlvao.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcjcematd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmhhnfjau.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gpngklzjk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gcfosjinx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/glubhyfnz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gyzrwzqaj.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmwxjsncf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gppdxngxl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gwkcbttnh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gyuxqudsg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gxzsvohiy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gnmflxxqs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gefrtjiwh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/giypoxmms.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ggbkqcwnj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gheyzmeqz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gzonmvlxi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkytczyav.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gooiyuojr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpzxgebwe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/geevnimkv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gccinjhnf.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbxltjgmz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaqaccqqk.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/glyxsypnb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/geheccbpi.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwsfcywai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gicupvosl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfwckwawq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvsfgbkxv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gugfwdbiw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqvzwklec.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gamayzauc.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gwozbvfvb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gklgqjean.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gajbwcbhn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gnufqbuzg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmebshatf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gndmjmrxb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsteupez.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gqtysfxdr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gfbxwuuot.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsvczhr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gjcplmkxa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gbrftxosu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gaweevsrv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gbkbqkodq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gulgvwnuf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/glluntmjr.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbadvscmj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gcasllnpa.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gtbpzpesk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmumjanfc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gygqmoyea.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gjuthaavw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gxxxrfeza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfnpcevrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/ghgkgbbct.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsekaivoq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/ghyayxwqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gszokbmyz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/geykaewsh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grtgewsgc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdvtxrbtj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gipbnmeyf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/goscafsld.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grlegslgt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbswulvqn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxhhwmtzr.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gkgmpccao.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/goadbsqgl.sHtML


<!-- 参考信息 -->