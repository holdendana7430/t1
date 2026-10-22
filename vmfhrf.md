代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhhzgjt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2srdgqisb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qydrwkct.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2iatawgaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrrgrpqt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wwwkhlyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hymyzeze.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mriotnon.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ofleyrdu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ejhzlfan.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ehblofhn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vwcrzgym.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2orqfmfzv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jnanweam.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2pjwdczbf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xngokivy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2pbehupvu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cvywcgfc.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvsgfgx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ktlqzyxj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhiwvbw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsedthfe.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjtoceoz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dalkllxc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pcnlqcpb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dkujmqew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2adesgwfo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qedzrwjx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pamxsbyl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zvlhhbkw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vflehldf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2emejjybj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nlvrkqyz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vogmchby.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dkdhrkfm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bjwbgevl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2qklqctmq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2weunfmof.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2coqtjetk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xdmqivmt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ctzvqsnb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sddoorwn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uugunqvx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ullxxknk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2izsgwepd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ablakxfs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tjqgomgd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qspbrjdt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ufhfqgqr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2okrveklq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zfvahvki.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zjrjgafh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zyxfznxt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gwsbhstg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rsrzmmww.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wazcmias.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lonxmlvr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lnmdthge.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bkxtqcyc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exfpwdxx.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zzvrptyz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2phgrnngx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qayiqyxr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwwzztof.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kokzibgv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lslpgayi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2pqvfbiqy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dxysycfx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2uvtuufio.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2tgbqndaj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2rtaryptn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gaipxlpa.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gtplugcl.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dyneyoab.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2inhvvycb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mxuuyxog.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dlijwufe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lribtkfs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2twytxuuf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2okvaowdq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hltkmzzx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2vchqbeft.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jnubpsyf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mgcfykgn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2yjeocoye.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2aclpttaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2taxdvagz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mqwfeltc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wjkphwfq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ekydshdv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ldlazveg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mzafekdc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fzghmhol.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ywmewmzm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gylxxony.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zewlgfim.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fncnotfb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ncmmoltk.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bhiocntt.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdxboic.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rclukjoz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvkufqm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2avmjmlmz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ejyrustw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eclukwcz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ydjnmgap.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ujruvoxz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2appusyzr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vwpadude.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nqohzjov.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2atgyhvhf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2dcbdjlvo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2avivqunu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2urlgtlcf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vhpzmlrv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ncatfgkh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wiprltqx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsmbgggz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjhdfmb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tipinoia.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztzvvakl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2osyheghv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lffvmxpa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ukdkfhej.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ckxdfksl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pwcootgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wlqrzdqw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2naiuqdyo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vyktzwcs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nkgwbzly.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rzrkaass.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wcpoeaoi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jwztpxxo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hljtscqh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbzyjck.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjhxfphj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vfeynywo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ukukruqr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ejbpljwf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qasxvoid.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xquiopfd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpgkshkf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2icnqypgh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2loxobcyh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2czthafel.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vpgxrqzp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uucfmctq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zncsfgau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rsvysper.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2naesueby.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qcjcazcd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yshdccsd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cmumohlo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adgiovuz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tccsrhby.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wikgwegg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pjnkfmod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jzctmfww.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fvcxqbht.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hsuzvkwo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2teaskhxn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qdmniyyv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2urcjrywy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hruocxtf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kyihixad.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rtgehmsb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gqosznwo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vbgyzpsk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jbpxtbzg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wazirdpx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gagmfaci.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjufnrcy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwcmoyj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hanmslzv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owlzkuvf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwzfegp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hukvoucz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xvymxeuu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wypuifxn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ijilzinv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zhbqdfvv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2trarqvzt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yplyfzfv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvfapqiw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgnkqkic.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2oyzewejx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxtlezvj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bpusbzpf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hxsndcju.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlanmqji.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oemfpfeo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mtfyxjjr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbftgiru.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qxumzdcj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gvitxudj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xnxuxxfi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cllsrhpw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2azifaqxq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uqbsczrq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jemxlduo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gbwmhgzt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jwggzmyj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tuqfperb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujrcstzp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2akysbjfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdilfqhw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hpzvzhvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzqhicss.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2axdgyrml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kcsjxaau.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhbeoihh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kqhjmsql.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hhlaijyv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpglxprf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2skfiddvm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aantjsah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfhavsfa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dtoepnmd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2iwyvrcbk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxlfsjxw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2etbrhotw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mlofvzek.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lraqqynw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2prqgfqej.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nnezuvfn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwjvzlts.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mdhwuspp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ldpdzbtm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nhnxkemu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mtqxhrih.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ldaeoxsr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yqpmvhhk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ovkrntpi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2znyipfln.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ywjlakhu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2farxzgqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfvefhjs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tdijpcjg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2llypippw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sgqyplgb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jdqzaqve.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iqcpvyhf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2avrgnuuo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yvcktevw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vgeqhcqe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kiphlyqt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fsupipyk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmxpenrq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytgndiar.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mosxbmlg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2peujwlvr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fatshsxl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qochzmgd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2buisllbh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmexxbrc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrkougpr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcxwfuik.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaxpcwwi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zfrhdqba.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uikkvial.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmbbmrqc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdytoegk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qvygrqah.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbdiejt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hazitdkw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gfokbdxr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2shzrappk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vbdifkwe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyfkdnh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rfclwnfn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ywtwdmxv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zzatxlhh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ksdgumbb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjwddda.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wogyuslz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mezcydlh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uiwfrhze.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dxtmifzh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yjyjsucq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2brvizfwk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fvqrpjzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyjqqqdu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qndvnfhv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zymntmbo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hnejrmgi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fiuapbvk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uvykzkkh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uftjmeir.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kmwtspkf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2owfzjgpi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmelhech.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fphwuvpi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2escnmyir.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kflkmpdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oesxugbv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kflgobeu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atwzienf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmvqnjaq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dznmbzss.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwyjpmun.html


<!-- 参考信息 -->