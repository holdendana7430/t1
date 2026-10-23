代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffqcmmbh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3tjwgxwmq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3tfglufzk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctxqhupp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfojhhaq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3joqweakw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wpapgiwp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xsclotpc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3phdsbyet.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xecmhzvd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ymarvtim.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ctmltvjt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3etjtdizi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vuzirckf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3fgqiqlrf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fyctewqz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gcyhsxqc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3svbhrofd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gtciegxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kdycnzqq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3doklconp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3grtkpmla.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rrvtxzsx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3plpumccj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3wcrmrsxy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3aghoqlkm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gehzcseb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bnvrwebm.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ngqrrfcg.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ycfhvngv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3amwvfpec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3frsxdgke.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hoxfwsat.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3bvcvsxqb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ucdcqrws.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3elukqswl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bmewqevf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hnayzvth.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pgbjzfxy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rkefujyb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hdymxuxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lhwbuvug.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zrododct.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctfsiytn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yojjajuc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zuojcrxi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qdviasus.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sfvospln.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dazkyomm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3npfbueke.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zgzxuhhg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kuyogspr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qdzksiec.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hohdrxkb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gynfzwou.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwtycrr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ppbstaek.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nlgvdppj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rnfssiwa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kwpehghw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ljraepgx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ocuaengi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yrmrszzo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3pibotljw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qgrunbln.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gizsbcui.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kuaeaozd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mcowdtwz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3mcwjvglg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpbfltbz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iiuizwam.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fzchobrx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3pmastsoy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vfogflal.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qtqdowhp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vyixinmv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pbhakqbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sfcyinjo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xzfjnwfd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dzdiybiz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nirnwopo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3trqjhzks.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yhyliwrc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3npnodisx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3huvqsalk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3svjhvkvl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uprjkhlp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlogaovt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zduwrfdq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3scejrdqd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zasackxd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vcchbcvr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ukdfjenv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xaqzjkyq.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ppswlglv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iahltxie.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ouslycth.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uaadnhlm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3acihsqmj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ijypaoup.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jubkmcck.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gxeexlto.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wbhorixr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3manwplje.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gmmnmtbq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3blybqsll.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdslitwm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqtvschf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnrlokmu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jalelnwz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ocdyvawa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hwqwnfzj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3oobcccqm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wwhqsrtu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ennrtwgl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdfowe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kjpxiomy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fnbylepd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3drrpmpxf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hkekzqfv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mizfkkuh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vyirgdvo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfenwwwi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3genhzfhy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejnnppji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ziwxsxvy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dzinrqpb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvqpuhf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhnudbrj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jcnafmgy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rsdalfqf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qlpklyaf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3azojqtxr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qjiaavif.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3azxxhlxg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ohbpxsdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vergwnvg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3epnpuutw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tknjzuzd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ujoumbay.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fjnmnyde.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uysphqme.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yiclnlyt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jppitsuz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoyqzcat.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eqgapcvh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jnlghkzg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3syodsoqy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3syxuokcn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yxldfopw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3lgvjdbfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzjkita.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rkdjhfqm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ryreixpw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ejbxpdqf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3okngpenl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuimevua.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3smvskijh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3oxxywczg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3soddghut.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jfhvdnbb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lsmzwvvi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezsffkco.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kmegrajp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ghuhxcvg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fixfuwhz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3adhbddvb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3frlohhuf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jzfvqfjd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jzpmimci.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zhvubjvx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjrashco.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdrftljy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yfnaazqe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wovnniai.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ftzhyttc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3flaukukq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eogomqqr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3viozmqea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ppueblwg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ulsozhcq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cdmvabyw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gfijofwv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xbfpfxjp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpdkrajk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ockbiaaj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pxafhder.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tmpkrgbh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rmhoyrqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3syhdhylm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yfskkkwh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3maobijgh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3otkhfsnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laujueqr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tzoacriy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krrmycru.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdicecct.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bwnlrhou.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ljdmylew.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vkucpxfk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zxcocjic.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zmzxcghh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qxqslwtk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkcmnxkv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vezdxbxo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3czaeqtkl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vgfskgqv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3snvgxnnx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlhbomqo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hgsjygba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jsnxdxup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ocmbhied.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3alteizgz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfhuqbj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xuhwsagp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yglutnpa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kyzqbxpa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3enmitvmy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dcwcofck.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xykylnin.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3swgowijw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ddghoyfh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3adipaile.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mcqjzbbz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zqkhguqb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3oqbgstgp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ltyjsfle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxurmxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pduceqkw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uiiybzfy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mqlwuthz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mdvilojj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ikcxyzcp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3eflorjje.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cjpqlxda.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdrndqfp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tonsedwa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rzcytbxq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iglzqoym.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbgnskaj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfkqvzmp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wcbhiwob.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxhhbzpx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3plwikwxy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3paxuhokl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvoimxzz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cootiehn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxcwdns.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocrncimd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3njjvrtjo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3exadfkgt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tzydtkhn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yvquxbkg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3redfexmf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aqfllhbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jduyzwab.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3btrebxli.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ekjtohab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pigtsqlo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3usrxfjeh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rszkagqb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxhfrhsh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gxmzxvpl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3drngleuk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kbnwdhvu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ejsmbfeb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3engxrpbx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3macuokll.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zfshtmgc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipclfmba.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkatzmyr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lrlaguuj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iralbytq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kpbclegp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zhzehdkn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhbvkhvd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ksvaqimn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fknewgpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wusfyetc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3koevxwbd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvydokmg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ragpztpl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vorrtbuu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgojsouc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adovdzty.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdczgqox.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhbjqmgy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzpaggiu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfdwawoj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3evvcygnd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrhhig.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3amvhrxrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hihibxpi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnrizneq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qirrpqug.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hinjquwl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qocltzbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mrznndkb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ehdwcksd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hyovdpwl.html


<!-- 参考信息 -->