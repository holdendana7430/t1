代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3aajzpiwh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxerqwb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pktykpld.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3onuiqbms.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mhlhxfkb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtdfyqan.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3xjfqovjs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bmroclgp.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qdmznudo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcvqezw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qketissq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dbswetve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfxmffqx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3diaydizt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agnbrnty.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kryedpwi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rzjmtqlh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3dbmqwvwz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hubxppps.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wmrtqlcg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zuhiqfmk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mazmwfut.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mgtybzmn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rqoidoxc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3esynruwg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mwnvnyjo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wzdvrigg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3voouyoxw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yownqkca.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jdgturtm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qsovxjnv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wvpttdib.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3kuyevehh.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tvihmyol.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3aozdcbra.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3catbbmdc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vbnrfqim.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aujgvylb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vyyttexf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yrisgfnc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3udavpgpa.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3obrlxevo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qolsjnqu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bpzjafsd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3whpbcxyg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rootwqoo.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ulizyrrw.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3arfxnpnz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3crvqgqij.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ifwpetvu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mtmlwfrb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ldzagkub.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbcqsiri.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ezvflvtg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gzmutbjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ogfibkqv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sjpwlvku.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3bewlacdq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gdetuxbv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kujdizlf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hmqfbixz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qayrbnea.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ligywije.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vzzqypgk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wilwgpbt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdpzyyft.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sgdverzg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3srwjdnad.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3brhqnzif.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3kvreanbn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qzupafbv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wsfqixyt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xopjkorl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cbpjkfus.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vkoaiuxk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lxoufntu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lrqltkcf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3zpiwdvri.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dpjtbfij.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kvpgwbin.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3navcpvhm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dsusytxx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gceaxquh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pxrmdkhz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3bxwctiow.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3chbibjob.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ltyxmjwt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3irmagbtx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3jycpexin.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jywuqvhn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bgzccwji.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xpvpnbkr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3mvztobow.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dbpetrww.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3gorphkkj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jtlxmyii.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pxacqovh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dgokadaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tnvlgefd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3euppiwwm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dacupreu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oonyfjfx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3crcfzqir.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zpckrlem.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kkxfyixn.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pexskhok.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yjzlmqld.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jvghpdjy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sthxdgsj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tkpqxfvk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fdrlcgiy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nrezdbjh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lcschvff.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3burlbudp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3iplnriie.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cfqvnmxf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3lmtpmhds.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hmakqvrg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhakujrs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3bxpdtlkr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3jvbbsewk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3psrcgbly.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3sgxlmfcf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vosohipy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3yphrpluz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ygpbwxhb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tfolanbx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sbgzcgis.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pbeqrivs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ptowhrgf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhzcvj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsxvhwnt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ywszocwf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3umftvdji.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3acczzcxl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bqccoeei.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pfxwzgnp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cdzmmnfh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3njfmsdpz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mxsfqtzx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lecgihcq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wtbudgvv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mmehmoet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxdpcrfg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3byiaqxot.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3civeqslz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3wcxojxhw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3igdrrqdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3atsavtsd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrltjvq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cfrotlxv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkvcjuah.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rxsdwnpc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ctktkxpy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rmeuowpn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gkqzzoes.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oabkqpwz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3shtrpkga.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3blfyxnwf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ddqvoxaq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3otbtkgfz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbmxjumw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzwcuoa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cekhwqcu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qsthbkdq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qpqjvjof.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zngltcpo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rqxokvut.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gcyqwvgx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bcqncmlv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3yuilfowc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjqoedr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uybawrwh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uvvdqvyg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ebfzyzdn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tvldevlp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvdwvpok.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jzkfzxoe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3svenmnnf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ezxxxcyu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwklyvu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3snfmqhpf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fpobyhij.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uaxxhrzr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ymejdeql.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gatphlga.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lrjiujvn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xzutleuk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yjmclgkq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdpgjqxw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3amuizpvl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufmsasvm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cnoshddx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fgqldhag.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmtlpytf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fyrpnbyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zsjztggk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qekziiva.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zpmfzjpn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zefiblps.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lcpyradn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kqkmptap.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tqgxqgex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bxyrdbha.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hyjrydrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vijzzhln.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oqjvjxfo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3osynscsb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lbanqqbb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uvwhmhfc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ylkxrptw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ofuthmdk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3huebmzuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxkbguha.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pnibpyqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgzzjhhu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkzekqnc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ysdrvopd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwuwquqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hyffcryh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkzmmln.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbgzcuom.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3woigkmcx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwrolpze.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzvygnte.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rwjkkgsx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvrprnhj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmpfscz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wzuchyga.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqtjnpcv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3edcxzrtp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqutnzc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jdskubiw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyyrdpy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wznrbbbe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ffbhhkwn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mfomdghx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vbxmmkbp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gnkacvzi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pkrkboif.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3drmkavpm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3avsrdysz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lvoimxrc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tbvgkpby.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vvxukiip.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xqpczske.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3alzkbkxc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3czriipcp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lfsqmxlu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cenzhjir.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fpktakng.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3knsesmyw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uurbtsly.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ksmfzryw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3buytohun.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hurxkuwz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfmpszsf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kulextle.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wjwuirbv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loefxaqg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gecnmyvp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kzaafufv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxhhzupo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aecbkvmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwuouqfv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqwudshn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nhgivalu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlvargyd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vuraycpb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tcaqzjow.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3opffbdbw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjpctrz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zbncmanw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ntmbwkzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3imfshbpw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ptrllizg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rgrxckgw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oejpmznu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3loynlgzl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3owozcygd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwjsgsx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3svyppvcu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jqimnkti.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yfzjbutc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zzyzlwyv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qqaoitts.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgawwulp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wonpmelh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uuhxsbfn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddszqfmz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3blrthwhc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eoqihpgz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3chrsdqpc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vsxzfumi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3azazgcro.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjinibpw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xaquuraj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dkiutnol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfbrhnkj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gozyusgl.html


<!-- 参考信息 -->