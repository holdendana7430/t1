代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2avwxozbr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rhtuqays.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwelufbo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ilugjgsc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ivkmjsqr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vtolwbvk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2srwkjvte.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2oujtcrzj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dbnmccew.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jncibfkr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2afrokjqv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xauanuxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceflzsvj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kiptappa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dluqgiva.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmkbodeo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jtgjlzfr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ymtpkzlh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2leyhncsz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rzmzprnu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hcpxzetu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2ycmpdwwp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2sdtxkevy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hiqqddzy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2updlhbrz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ugzjfiem.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2thhcsiur.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gwlommrl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ljqxjawu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uflxezks.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jxlpjztr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vozanrjj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wjvuheun.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gamrzkyc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2eaxhntip.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vdxizzsd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmziuajf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dlnpgxwy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fglbixkx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2prafxvvd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2tqiolzof.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2unwwitrr.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nigdxult.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zwmjvgaf.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2mwolveex.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fofahfqj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvlptuxg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kenmilhh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fjbmfnia.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rphcgbgh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2undazupm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2bgasaqzs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kzfubldf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vgejckjw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zinbzqcp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rryeklkq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kodzhcsn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nouwipem.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2olebpdwh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fxznvihy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2evsxbldj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jskfcyuh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mwwcgxbt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iukkhocw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2puklvxht.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2seheccsi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yahypvqp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2attyrxve.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ckqvmdbz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2eiddkdvm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lohlbhaa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2adehbxhf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2voiqaghi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ttnkxvij.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pctwsqyd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2oxnzctoh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qkslldzu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rdwvazyg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kebcnfbs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gmdgfuet.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ydsgskgk.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ycbczcwm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hpetrdzh.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yodzrzqn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqqzzcdn.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdicjkog.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2obmnprvh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2rvcwjxbz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pshuamfv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kpmhcmxf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2czmpfpxz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2gjtuxwfy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uxxeajft.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rkplnqds.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ozdhpetm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncvmyaal.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yuvvrsqz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2crocujyx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2oixlnova.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ypoqpffm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ayxyoogu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bblrvmte.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gmabemye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aykbqwyt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2wzlqywxi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxikokmh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jhdswykx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuutbtmn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2euzbisuq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oainagob.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jshwastx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qcofqohx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wjmjlnum.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wyfggniv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zzjydjek.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uyglnaiz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lzobnkfo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2frxebyjl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlxadoly.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bpnledca.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2egjuwill.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ruzoxqny.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2igecyqob.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jopldmhz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvriiyr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tzqncdce.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2phjcgkgf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgeylmmq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcuaryiy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pmloehth.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tnyysgtf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yffzhuwo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vsoyaffk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ausixuoc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nmhotqie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mitovakw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tejotnch.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vittjphs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uyinhxqf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjgovrn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lyxsgaqb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2eygilpfq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jpohjlpr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hufzodab.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jhefcebw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bfszyvpd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2izsbxyrp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zgwdjeoj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhjhflb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdewyijp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rpmlgsya.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2znkgqnma.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ohsupbri.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dmxekgrp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jojrbetm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzcouzu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2poqhyyhc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hojyhemu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2djytxqwy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2raeqydup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cehetxbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jisqsdgb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2emenfjfa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sjsfcmgv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htfchwbl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2djkntzkx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2labfduvf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mxqmpfxk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kbddocay.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmlisdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xuhubpuy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zttwijhr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gbzunlyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mnqrpxqy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2genuwckj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pqjkxzqt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2syshbivb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gmoufene.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2saycqfmf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ynyyedln.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kmgqgoaz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cuannlku.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nxsnrocj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lnvxsgib.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xjxwgeee.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vdqqmcty.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gzcttdzg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yaltumxx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wzijayrc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lhyymtmu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vgnnwxye.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2obrzffcc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjgxzd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cdganuno.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxnlymaz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hmikcula.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2katigbkz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zfyqmakf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xqozhsfw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wbkakeeu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vhenbekh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2snlxsttm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mphufarr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2itdcefrz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kzghzucz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yooncabf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eyveqifm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nccowcdg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftupmkth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2toprlpvz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tvtjhitk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bzahcfqf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qykvstki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivraajdg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lciayreq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlpyaxpj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rtxwijtv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ftaqfsfr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nptpgpau.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mquvviui.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zhtlszbc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gscluudn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2aruqjgtk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmxsttsb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ipwlkstz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqzodtwa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mwsfmiyz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hhkaellb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vkmcrjys.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umbjynaw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxbohrg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kkhptlkx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pcuwhaxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2htsjkclq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mhbhpght.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zdhentqp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zkpbmczl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wodboueb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2upkciwta.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ovkggvsz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jncteirk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2izubgmmv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wcgnpcql.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnlfxdve.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2onckwmtt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2efuoblnx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tkfdijon.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2scykwxbn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wotpwthp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qbitcnch.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2npzyfoew.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zouhwour.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qcnsxbgv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2migdixxg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fhwmgaee.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iukaxdji.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boufdhbn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2csotqurn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qvirwuec.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgymdhcb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcrzfsci.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhhyaveh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ooprbzks.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sgqosmbc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgvrathz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmxlclut.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvktyuuj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcfxefjj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unxiroti.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zisghsew.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yowgehqz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ougumvho.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lkgwocgs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aivjseqr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nhbugqjy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zotwzdof.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2brjgdnfz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ilyvxspq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rxaamkzk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cnsmycwa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fvzpdbcz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2agdffdxx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mbooqwph.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cizlbtow.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yfwwcaaw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ncaztglc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gvwqdouz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2puchoayy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mkzwhjqp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vclppuhz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnhdetrm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ygxwzomc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nzfvoekc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mkjakytf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jnnmjivx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvrymgaj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yuughtlh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uwalsfns.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxtnctfm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wdqsrjdh.html


<!-- 参考信息 -->