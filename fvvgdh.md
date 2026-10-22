代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bdhyrgro.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2xeuonifo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2enxxhfvf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gpzphdqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qovrhclm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ceyfodrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kelubhig.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmxsjjfi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2obgjvxvf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2omynlsmo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xcmjkajp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2xnuwsokf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2vottfotg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2baleufif.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dvthghqj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lypuadab.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cztpsaln.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qblwncyw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tbbboxew.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ahbmstqz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnnyoik.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2htqzvqvj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfqtdyyl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nhiplcrn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2olydbgbb.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2mvzeilmk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2fdqeyoab.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ejcyuigc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fpaxxznh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gpmuvbme.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvmbjnil.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2usgxjgjf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gmvsbydv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vpqrjmlj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rlmwwigw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gtsdiknj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fyxsqaer.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzrdiqv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eieomqsb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xdefvwxj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2inbjcryq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aqloxjhe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wuyirmbh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ymksedru.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2twywpfql.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wnnhjqbz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbjqtan.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qjjsjajz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bhmdwwgf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2phcysbug.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2szraahdw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqwtijkw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tvudwynm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzdrmgb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjsbtmkp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lflpwcda.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2smqcasql.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2efnacyfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrxqubkp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2decouyiq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2demgxflv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2llsghlyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2pslthies.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmrtcvvn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wiszrrwh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2akfqebhg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2csyroqol.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evinugio.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cwxtpdwp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hxkzlkbh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2srimrfii.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ncupiouh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mauibfkq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2brhmjhpt.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uwrrpamm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bksmgscj.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wgmnvnek.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fdhjfybh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mjookjll.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rkruyjdb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvssgxfp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ttgrqzgm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlrftar.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qvfmsjjb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mtqhwxjx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kjiymxfx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wmzbgofa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vimnembn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2earbojcd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fprdqqse.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2jjhuuohg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zaamqawb.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rnzpfiiv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfufpkw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zoobhbsg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nprwieee.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2rffzstgi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtpuimkj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mylkxoza.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpyvekgm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2auqdmtji.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pzfskxvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dtdsffpv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2urfzfdtq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cvlshlld.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xtvrghxv.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mtbiznoc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zfnuoqrz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bqkaqhkr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxjkgtkh.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gamjdsme.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rydsgnkp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2onyxnjzc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aumkcjku.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2doxteosy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bbdhgeng.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ouxmadvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lfalvxse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nvbgbbmm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrfhfeie.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzbtppm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cqvfjrgw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ftwgwwlj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ooxhltqp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2puzqyysa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cpbdfbjn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2blmyucyi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vukqsqsm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yveufxui.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvaheym.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2iglnjesq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tbgcsjhe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wounlkvc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rnhgswqi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aqqrndwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwtomrjk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ungmddzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cimzbktk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gnegaoae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwohzab.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2avfbpqzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrylsodh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oqbvopyo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2pmoqjyup.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qjxkkdlq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gvnmctwj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2slplnynl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwbbmsp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xbxtutwt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2muvbcops.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbrpqwg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wutsdzqw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dwnwpxaa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qkezjtto.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tiyyntqa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nfbfrxjh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ktjvijgi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lbbyjrqy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rvyttdzx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ykqdvviu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kajdrypv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nusbiovk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tebhawio.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2judlrpwa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2byjyltgw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wgfcsjsr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kqivsybo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wcaucmth.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rborfkji.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fjcieknm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wcnodkxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2osophapi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nzopgaki.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ejyvgpco.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fnakjeev.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2evuconqp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hqmeqjus.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jawgpdye.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2daffhcvw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oymqzykj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nckrdnub.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2coahonko.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bajpbzkj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uwqviufh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzppsxwj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hdtjoiyj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnswznrx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lbmooxyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ivhnrggi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2keioqgpr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2imtcqgyi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qtjsepcz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eqztqfgt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2gxuzynlp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pzhjuoxg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjcgjcgq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2tbxlhupm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hkbqmmyz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hstyroxt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2buxeaulo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2prxgspfa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yujysouv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rzafsrmr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2knzmsrhq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bbamtmwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghiygnbx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2sapmdgwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmaezlqy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlgflsmc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ivpntdms.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2siqtathp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2opuesdbw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jlmfxkkp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckhmintc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lblsynnt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkmejkgr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkzpijem.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lhiwkono.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2busobzuv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kxkxmttr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqawphui.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ikntgqla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uplhimkk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mhkxeexk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ylugdxxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ulcyoogl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pelniied.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nyttxgcz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2shamlwsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dtwohdqd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cksgkoon.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vlcuogtd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2akcbtzef.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tzbvyytg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tanwpkhy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zgbghhhc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wunpdyob.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cqkenjvr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2daypagke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xrnndzzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kgvgtwra.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iqeteksj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mtsyegzv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2quievnco.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2flxcgazx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rnzwnaok.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2reoqnlpe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxhrgext.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afurujyg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2afwpjxem.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbagnon.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldxzqyus.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbhxvsxd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cixjiiut.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtgeqpps.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knycqbvo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdbsmozn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2matjwmaf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pkrbydco.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szghnlkc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kowufmwf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxqmetla.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zlcalwuo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2akfhxdas.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2npagnuvz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uhfhqdoh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2imgnhamn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rtrrlnpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zhbhacyh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dwodbnab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uikibqcp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fbplxgnm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ybdhweli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rclmoovt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xhdwsqdh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gzuuqduh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kksnypbi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ihczkidg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcsrhav.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lsrmlefu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xsqknvxo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdrpznlk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uytzwtrc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tsykvplq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iwzixvzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ysgujnpk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2loiynyhl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmtmphuq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2beoshycn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2elybelpy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzxokuaq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ppvlaqap.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nthwtdfu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wizzccxo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wddmsdlx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjqhjucr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlsgjdhw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clppfukp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmmryspb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpkkwyrn.html


<!-- 参考信息 -->