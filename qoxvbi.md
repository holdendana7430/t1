代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gwhqsajf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rhrqlmmj.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nicvsmkm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cnzmdmgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlsfdscl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jekazjmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvrtodqi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zlbcoxwq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xkqrwvhc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lyzzpepg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sjfcebaz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hwantbrw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkitccwk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2juceuaon.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2wousifvz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2enyepywv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ofiggwlk.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jdvapgdq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kgufvzyh.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mrgybprf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jsdicyjw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nrieirqs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cabjvjdg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ykhtcpih.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lvtzponv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2weciwrur.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qxwmrbkd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jcxmidud.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2heygsqqd.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jvtgdjjb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hkjowznn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2pmqjbzgk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2anbtunmm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2nbruiefg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2laulffrj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xhekglyk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wrgfhpeg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lsftucwu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qsyndvml.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2skcxvqpg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2dafcolrf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvcppyuf.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sehmghxz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gwhhdkky.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fpghcnls.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2vwxuqejk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bpjvoojq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dffnppjj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ezfvdxhq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2eyixcjjx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ajeclvag.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jqxbodwp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2okqiobps.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bzodxrie.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fqiritvb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rvpjycdu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dgepxnqa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xkahbkhw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dykkhyqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mnouuoxz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjhfesj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pqxfsxzz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ebckupwk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sdfftcog.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hjtfhusb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cisosanu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pmlslzav.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhsmsaa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jydqkegr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jauocrhk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2eknozcfm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2oqwwzwin.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2unhymmwy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rhwprtwb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ylziwrax.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qwiyjohh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lexlaqbw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ptzksrra.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjszwge.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yadojupb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lufxlecw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmsywntv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tznhurmm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vckemjov.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vgzovcyd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2oyrjnhpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2divbonhu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bdxddkwz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rhilpwkm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nkvnnuiq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iluzcdyu.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2awjbmwto.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aormkcnc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2voryfutx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gumcmtdo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bjuzsskg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2wkbquexl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2lmhxwilv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ejuxgxac.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2enzcpgro.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2beaelgba.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vssxcezk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aorzxqak.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qwgfohmp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gzbuyiat.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2koaxudca.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2elxdkdzq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gtyjtbrw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rcieiuxy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tesnhpkx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qkuypymf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2uodlihwk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2yciqvedf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2feypchfc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vrvmmknp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2knqkuenl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2oadkthif.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yufejbbs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ahdxtjeu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbfkbkt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wubolrps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2axaqntrd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2dkmssjhx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gdlpqdxa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lruadstx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wqvmsxfg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uafrgloi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zxzukhzv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ywjeewyn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pvkywibr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fiahessz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2udtvotcu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pyrxdsyf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eizfwhcm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2actedlgz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kqoycgej.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgkallgb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hjtfegvk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gbfnrxiv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pazgyxzs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhntfiy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jcocfwhw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kdbuzxjv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bhfrmkjh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bzusrzbs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ugnjjnra.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wryoupoj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2drphpcfo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rjbvaamg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2annfehzh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubetagzk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2brtnkeer.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2etodwpfh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmedobjx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xvkprzby.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdyuevct.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zunfojlo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nrwcdgld.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yhtlaqoe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ijefgqfi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkyloqzw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2edhlcxip.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lbkssqjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjunayqs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ydzlughu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ooylhedm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mgtyvhsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lnqevgov.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qvcqgwxa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2avqumniz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ffrltleb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xekuenbg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cquyfkfh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yvbyizdt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kqdyxfmt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ygblhwqh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tcdkdklw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2iuixgmhu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2coyvwteb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vvfsuuef.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fffsafmt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bmmbodfi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kezxbwtp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yloylubh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2truderqh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2djlsjsqy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieafxbrj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ffrqcnja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bgnaavrl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ktrrnzkw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oepmgxzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gzclbgib.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2znbexbgj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lifqgvel.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cgxdwdnq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2viyvoiam.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rwwtzdcz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uupeeikf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vqlihgsh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2umxoqxex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dzhjdsmk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yappfqyb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mtomwoby.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pxcrjsix.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zskfgacj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yigsmegc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2okcmpjeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kagawqdr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrvfovhq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wjmfuyjc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hitsuaxc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2btukbjqe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2awhpbuzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fvlybrsh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hopkzemd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mobkzzuw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnwlukuo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmrqjdqd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qzwrbvph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kxdysvsz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fqjikyvt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zlklwuek.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fypvhssd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2osdlauqd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lyuguzvb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wkljzlcy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fhuoqtvl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2znznokwg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tiehlfzl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2visccqzr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lwapmfdu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xltqajnd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gysatdgc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hwyhaflb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mplbnebs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qertkcyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2imqitceb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dkczwfwe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gcpffwzq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vlqfcfhe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zspdqrpf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vtwaiyqm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfjnxcx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tedluqrb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mzsengtz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kgkxhkuv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egitsbdk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fykheybs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okupduts.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2txzhltzv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uxoquewe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zthmkohc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtysxphk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bbdvlcyi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nclpkjzd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mtbdorde.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgocymba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eawzpkth.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lpcjqdry.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdgixudl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjvrsjei.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfjtehmy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sdwvjrrk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ljemapat.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ujzkjpsj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2atqghqry.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tfaxmtyg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2oexrxpyy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wjbnuchf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vmntzqkn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rsdqisng.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vzudzlpu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hlbicdwt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vmksyzdp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aoxhnfoq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfztuft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nasiixyb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2biloczbd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pnxeazcg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pnilnmbm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vdhtuzsj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcnlpqiq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sganngak.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lpcujsmz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tioekrfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxuzsddp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fbbdrphr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlhivogw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lyfttnzi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hihemvbm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmwhgxsu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oudgajzo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfoduhon.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgohckxr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uqbcqloa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqmczugm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whunkkcg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqnnfsog.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gcafeljd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgmdnji.html


<!-- 参考信息 -->