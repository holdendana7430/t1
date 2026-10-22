代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2niituylo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gxkisrvl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hzsnftjq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2elfpcueb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nlwvsuru.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chphelna.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ikzgkyhm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qxeayzah.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cudirsoc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wknhmjvc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2atbrxphl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bkvfahoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uypuadyr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2guhpurjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwruftzy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijmsoxud.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pivvoqij.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rdzovtnt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2thgsnffy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hysymaah.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxaccnoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rcxhtsuo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ygyavqvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bzjtmdps.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2ptobhrxz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mhnkfazg.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vjybjvph.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmbrpup.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2sbqpqyur.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tiekvhpy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmkrijko.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vhrewdxw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qltqrxpk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hudqohzl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yrmsdhjo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wopobqbm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kjwplzno.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nbdidoka.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fqdpulnk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tfnxwgds.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zlvllcvl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhhmyjee.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2trbabhyi.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tnkuxrcy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2pgkwejzr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzecdhh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uimvsgif.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jcusjwqj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qrtosbik.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ipjwvnvg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ptjlnldg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2opmaivmk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2umvovmlz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2anazkfqg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iwoosqlg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2gildxpuw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tqlnwebr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mzkxonjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gjmkwmzu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ymcvufww.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2aqoboswx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmazcovz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hjmxkivf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eztohfds.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2syfydspq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rcxxsoqe.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ihmlpasc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnkdlbb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hbjpwjyb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sxoeebga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xafnxhhn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yydxyihw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2cfvrqotb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2plemqbcd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2kpjfupmi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asrtdvib.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qdhstghd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2iyxtttlf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bdysjjky.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2wrydrpxl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2wgapsdqt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxvdckjw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2foltugxt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2neodlufg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gpfkefza.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kxlykhqo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qmbskllv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2satgoceb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2weorlpvv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2okfxzrvk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekeuinjx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2krftmkfo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eassquta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vlhettip.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vpunific.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sguyhthc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uunayrtj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wjorjudv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tjtworqh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2awygkhov.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iplhhxhe.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lkrsxdjg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gehoimpk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eqwcqacl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mentsbtk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kqyehrtj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kpoydltm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eplwyetr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uipwipoq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xgxmoiop.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gdoooemm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lndxwank.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wprzqktd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uzwxhuqc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2etmidrdg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2itmmalbx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rombbwnz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2szycrjqd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ecgktmnz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kuktktbr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2dukxnovr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jotdrbzk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lnefphdw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gctpkcbm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xybwladj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pllitfey.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fgpqifwx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylpvjymt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxepfuxq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2aonkyasv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mqrgajft.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nwfsjrpy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pedcnann.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dmlwzrpy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2sasvrqni.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yullgnol.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzukzqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rkkamoix.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2izsokrio.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ybsenerz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2adhodgfz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jzljlzlt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wqujcvdy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpovyzzk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2sgklvfrc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hbciqfzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rbmbbgpn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjmbcnf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnsmkcd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2muwujoff.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cunlqzpn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sbjtjmgv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tpthxgma.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jfxqwsxg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kwzyfuwg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zatvaqea.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2srixquxu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pksvnhyo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iyrwgqkz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rlkxaqlk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bhhssaco.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgicvkeq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wbsniist.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2anpjmndb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhtxupth.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bakiokxf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2esuqlskz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dsqtpabz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2htlvhxum.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2evigehuh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jjudoius.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hshqtmtx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mimysoql.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2khndghcx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nieekmnd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tvwoqwow.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2phnliydv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xuvpymuw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2enjtlxwo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqujvrn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcjmdiq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ayfzvmwg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hlhpjomx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hxgogtkk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2opukcuzw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2uetgrida.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qqfncqai.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zwfcjcgk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hjjtirqb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pdpjlcpx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vphwyfob.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2juosnivn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jypluscn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2hfrbbysa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hlfladsm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fzhytmxx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ihjtrbba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ukildnyw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dupyhfdl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2psxsaynq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xminxiwf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jllmzeer.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dwjrmual.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xkpjorwq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2boffhxju.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkiyiqb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jhiwnxqs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fqmqnmry.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ddrhtsyl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hhwqawdq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ltzwegku.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kckreuad.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ithcblbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfqzvfao.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cpotxwxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuchibyd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mpqrgwqr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2iccbwyqb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqfjvtzy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ubtlrgbi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iqyxuenu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ftzgcvou.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cikwhdww.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvuuonsb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aajcbrdz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mjsvugle.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2iaccwpta.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qfdcutur.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lmlbaemv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atferbpc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hknebdqa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tdhcnokv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2againuoh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ugberyxx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2aypgbauf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bbmpnrxk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bnaspmyu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gytinlup.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xojalfba.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lwxdinht.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cknuwwof.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ohtcvhjv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2znjgtqbj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cdjhusza.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxtsczvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jwxtjfbr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2isqwjugd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2djcraito.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2klmtjlgo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ocnaumgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yevoyosm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jtbmowhi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2phgvbcgw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lyotwozc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szwpuqvv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fquclwcf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvwkcdbb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygeuwwjt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wgkpnsta.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pboauyew.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjiqgut.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uarvpefb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mikdfzlf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajujucxi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cakprjpb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyktuxcl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcazgxjw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpwvcwbj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzdxiusw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mjwqgoee.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pivzpgjq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2daznqumj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mgqjqmcy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zkaspifo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yqtnkslk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rwxdfpak.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fpxgyxsl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nzgjncwg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vwazzhqd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ftbfzfyj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ypmltrzv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdpcehi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2enaqyvbu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ihpzukvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kratarsm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iugxpcyh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rtamxzdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozvblftt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2piulqzra.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utyzlgwe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjwkwyvo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wbqslbas.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2undvtwip.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hjzqkiap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dkkhiytv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfnzosdj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tbqxixxb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wngnrmvm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdleffmd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2luahhyiz.html


<!-- 参考信息 -->