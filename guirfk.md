代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oxgslvht.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2hcayyhag.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2oeflzshr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gslqnzfw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2okfuzkzt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yaaqdgbd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qdtjtjxj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ymtsmfdn.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stwigirc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mdhtlyfy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvnxlydz.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2olsphaxk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2keexnhol.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fvctwdsg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zvldtynp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jxhblcjy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yhhljivh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2efemzjxn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2swchtjfu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zqfjvdub.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2djwgycut.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pctaevej.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsjzkamr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zftsiyeu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2oosbuzrt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvrgbodi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kjtejcte.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zvthsode.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wsgmafnh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2itwalkqd.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zktiphwt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfsdqwlz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2isjypbnd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2udjcvnun.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uulwafey.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2hwjsvzoa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2cjxzvndh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2fhydnkjm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pyijeuah.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ijsnwqex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nulmtkhu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2lqhuqhxm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xzzawfia.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vpatnttz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zpwfxyvh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dceisnif.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2tsmgmngu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2awsajtaq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzyscowe.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zgjqzhav.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhgyoyf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kozgiuoc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pbymvqdh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vujsucue.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2syetfjhm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2igtndwmh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qknmqqyx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2zcpuegsl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2snuaqtsn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rfzbjioj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2sfjlcneq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bwyyahwf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2emkmibhx.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2hrzcjknw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cqouetrv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2spctxbfy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gpbyfcpr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lejuozhj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sytiqptg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rhlhqsqc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2msqdijik.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2oyewopac.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtnojel.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2grocnuus.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uvgqwblt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xllorbat.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cpnvhule.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uepohrhv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pjaxdgts.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2uonfrzfe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jtfxcaxp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2scmjvlgo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2khwjbhku.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqqnzhti.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zmrivdix.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jwudpglx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eyzplcvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jmnyociq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ruvkzkpt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vmgqcqrj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xdisdzvf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xxmsbgfv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzluurdh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2leqrhrbw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2egtfniqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2urynbqkd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2emhbcbbq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2orvcffvp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ipmlycgf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tvdaeszm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rppmbihe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mrlljgvv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2quzpcsbj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zatokbve.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qaoriaik.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mxmmqguj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ufsutdhh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qudjtgzx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pxmbepag.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2oecyfxgc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gofzdbzk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgkwffu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bavynucr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hvtldqsx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlrezvf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmuqkjzg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vvkttywq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pkmbzwzt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bgdgdlxg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hucvfqgi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcsrvvxb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ualerjdq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nfeqarys.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kjkktzex.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jkpujcee.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ohmdkxxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcmsdle.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kezjbumd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hurwsqgw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dwjwuksg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2espvduzw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2rrnyiqlf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gulaiyyr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvmmuhkw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wanjdgrf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qaibefbb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xvlrnoif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jnnynmaa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bmsgzmxu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fbklxsod.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kdwgqzjm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eaizrwja.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rddfakqv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgnsea.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rxcqurvi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tooapnft.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rtxqazfy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bexxency.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2viknbmtl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2sbqoyrse.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dkneevkk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2fsygyocm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2mtspwvwi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eqvgvtkn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bcxwohbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dihefbzv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuussgz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kotfelwv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdugvrzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2oulyupdq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sktyeipw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xeonbjwg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ildjxpea.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2laeeelll.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fjrpksmn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aqflblzh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwlnxfkc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wywpqqzk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ghlclecs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2obqeouvm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pszctypp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xeozlnbw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qhngghqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2svoklrtm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziiqjaqj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jymptagk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsafixey.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nfpuikhd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plhedwse.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uszcrjzu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wqjzspbv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ltxvueda.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kllgawgm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmuwzvbw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ksykenje.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2frfrvdhv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rixiriiy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2odgkmuff.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktrsqhln.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxifkwoe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ayovjcyn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cmufkqau.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fylysnom.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jqarruwm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gdioupwe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejksudzj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gqxwgltk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdfipump.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2iugruofe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pemmcfvy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2plvksonb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2srsrzmon.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilsgnqfd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2chqddtpc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mrdkbpkx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2blmfptnb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ovlgzfsg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnvyadnd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzlmwaeb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxywlmgi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xwceyoli.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjixkpr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mxasevee.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kygwrprc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hopvnqxh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uihfnwqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lompgjmf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsuiflu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2igpnyqby.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zbskcjxn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hgjyvfdg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cpgjuuvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hsegcdqz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cngppsfo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mdnzxkna.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pmbkhize.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hbjthpyn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyxshqqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jiffqelf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2friutmlv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzuuaby.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbwvntxg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kgfxuisg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bgfdppou.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2utefsjwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hxdlcbwf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ypectcxs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tzwoyobd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvxjjhte.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzurqvrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lavqirrz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vzghhcky.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vudczysq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukiuwqxb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fewitwxb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nitwfwfc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doyakccy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghlejyeu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezhpbdyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xspsrdxp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ibcgnqzl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwsmqsqp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrtxstlc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hmaufcjr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mbzaakzu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fhuasfqf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ggvmiulx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fimoncup.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sgpcxuht.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2znjtfixj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2aagxveck.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qqljtqeq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2arurviyt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kvxfujqj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jyimzrkn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgvjjpyt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gyfgjbnu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ahocaqou.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sxjrmftk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ppnrvlit.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iuxfzkxw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2agzefgws.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kehcwvoz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhldwxhr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjruyscp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rydyifhl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fdribubv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2svxlvkol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zeoxlngz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdeswhmo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mofcyzkp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lljrhoud.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkeoscqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oarkmbjf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wallbxwn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyqtroci.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2csrqrvpg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vamfqrlo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aegdqsmd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utxinaze.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ojvbbjpo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjzruvae.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qjyvelem.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsgxhrtz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycgwifpf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ioawmswg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2smreiudv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmqkzqrd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dsjvmczl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wjscoeql.html


<!-- 参考信息 -->