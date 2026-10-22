代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ztyvwjlp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xyihzesi.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ekotsqls.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2jdgffjon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imtjkcvg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2bxtdycho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mietajnn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sdelbphk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2owpozvlw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zugpjjrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2cxfcosct.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eprpkoex.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lswjpmfd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovmewqap.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2fikqlosp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vytubosb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2xxbbtugu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rcgibxux.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhrjtbl.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zeuadxvm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iqwudtnm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ugthgkfu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2thtedsks.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uugeotns.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2utxjpphw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2jlpgqean.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2brklpqrf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rqibspqv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvrwlwjv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrrhnkf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxadbdvk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2emdejmca.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ppbhzizq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmqpjyl.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2tfgajeww.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kxjnbcgs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2imelxnzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2priefwsl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tgeguwbf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ariafvft.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2crpkzcqs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dipumokx.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qyowovzh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ukmkoneb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zymxxszr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rlfkgwzn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqjlfnct.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zdvmhrky.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wfuvgdfb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bpfhhtjj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2pipeueyy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgrkytu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xhsqullu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhcfvgwv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hquqkoug.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2okljdsxm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2toaopjww.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2parzzkgt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlyqsxef.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkugajgs.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ygfviuek.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2qsdbujdr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ljgwjzow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dosnxfxf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tlvuzucz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rmtqowcv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2faichnkl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zvkbkinh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pjfasuup.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ecwxdbjm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gotekfir.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhnzvpv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eoilkpqh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hzufzpnq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bcbvatps.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hetfclaz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2sjrlylcq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cnrrhaen.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vzhnpkdu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2aywzapum.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxkluav.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ojopdeon.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgejey.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kyevmwwg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjadffqb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hzgprqaf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mkgurnxu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rkleoqdl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2hmdunjkr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nbsyyoib.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ziydfpzm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2donrkekq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2osyoyoju.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lzawvgqn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aqfafyuw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgiiphg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2axiramwp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qmwjfdgf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qwmccnua.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtxrkq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ecjvoxje.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ofkbixrw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jhmpeaim.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bonvomld.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ivmawbwa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zbpkwnre.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2djtvpqdf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2dcwgwghr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jreujjyk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hggffczg.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2azjhirpb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2fjokznvf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjxzji.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lcjkbmjw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gsxheciz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bsczazhw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2flthruap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqpxwwqy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qraqncvl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lbmuymgg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lexcvlpc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nzmftwhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yueyynnf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpnpalll.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2qtxusbkf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lcpclptp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ilelvntv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ytudawau.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jiyfhmrc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bixagfzj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ypzyshuw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lsjbjild.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2psucipky.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rdzjwrzq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eequjadm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2exzevuyh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nufwgwlf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2toruldox.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cnwzwyff.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnsvvsa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vkhwofqy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2brsfaksg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hgenobzm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2uplzhchs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rrqbgbbs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wfrhrasr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2joilwdfi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eizrjvhl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tcckbfov.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2irzcbhlx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dbzuesgz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mazmxdei.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2typtycyo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pkxuyczp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ehgslnnb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2riedijyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xbplzuuo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kgdipmwj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mxdsphdw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aonpokky.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uvchhzua.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wzwzwxla.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xlswvwni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oombwqrz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fwhrburk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oafouajg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gcjcoyjl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2akyrasil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ldeanvcq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2thxglbat.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ntquhtvg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gzxpfywe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cqeqtxpl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ziprimxf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rzwiffrm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cfvawvpw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nvmcmjje.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rvgujmnj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rfsmrtja.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xnrhjemv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wfxgtbic.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hmfofgha.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tfswskyk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtdqpgos.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hesbyeke.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zhelsxpf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhjlqsiz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2sauunhgl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mknkijax.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wydduxhi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ivjrzmtc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tundtniq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2usjcxskm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2klnwithn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vfxghaky.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wdpagvjf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wrgknwpi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbryrfc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ztttyfpb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fubmudte.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rzgqbdwr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ecuhfxdr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2amebvrvm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yrjyapof.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bawucgkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qorwvgni.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vjczsmpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvxqkegi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eevtuuto.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bxwwydxg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2leowtxbb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hwtxfzyq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2betgpfqm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iqjpeloq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hwflvspl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlipaoxs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2syxxvezr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rngnctzo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2majlhusf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2koiykpes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxowhfpl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrlcubla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hpyndqpt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmizbdmm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zzuvmfdk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tvwzsyuf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ldshgrwx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jqiaqoxc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fmzblbbj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zfdzlgjk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2glnewfgw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nsltpnrn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qaaaqmny.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2oekurzgk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2omcsrive.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2igrvitsa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qdtxppki.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fhdiatxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lujbuejo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tnbdgdjj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wglfdkjz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qitggxbx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2sxrliiij.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qndepyxp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2frsswynt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tejbsajh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aktwuvyl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhhwscjj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjllfrbe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nhilvjrh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qgpgqyox.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbcbdyki.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frjmttjw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lcpkhxnp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gasnnvbo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2npeodjvu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxuckiok.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqawfuvu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tcrehqaq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fendjwiv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzhhgmlg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2daafpvnd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2agipwanc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zcynnebe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zoegqpna.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ogaegcta.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oqylhpid.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxocqnjq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qbdfetbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iuwslvbv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hpphuzym.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dzmhlarl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wnfcdyjd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oanqnbpa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qaovzsel.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2khnvpnvi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wfswobui.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jvxhgsrv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zupomtyg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tnjoiate.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gguvgmpx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzfzxars.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2churcxqa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qnchfylu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gklmitlp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbuvxjcf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2plwsyeth.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mknyzsfj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kdkfejea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zyjrzobf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkwkijmj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cklkwvmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbjnuooy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgllmnkc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cdbrkjqs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejqzwmzh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szsucfen.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zogkptvn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cpjytmcx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2beltuyzo.html


<!-- 参考信息 -->