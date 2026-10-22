代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2inxcivry.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dkaveotx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kwzhtuyx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pgyzxfig.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jvquczqx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2xolojrfx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gjcyktty.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fozmazpg.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yujzvxyf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vafvewhw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhbvonsa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mcnsqzxg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vbxdsasz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2giwcgkrb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dmjjcooh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xxhhutpb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkaocfg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmmnzyo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rxbdwilf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrrope.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ftlxeysn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdpznbz.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kfqkmxoq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rlutjnhz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2cofypafr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2foqmrgst.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ecakmlem.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2opnbdvtr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zgepqvez.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pddimxix.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fpizjoyw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2btolfqpt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ernmnhpj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2eeljkmtz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vaurgysz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ivnrxxew.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gumiwpnf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdsmvwaj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yvtxyuoj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pwbrbnej.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qsxxnxtd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lubugoic.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ffuaargp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ikbwioqc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pdscyroj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gdmgsrgx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjddgbgm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xhjvzjnk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lwzoygid.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hnnanxmx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2syufnpww.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ktlfdwbh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2bzaajmwu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nklhcrjj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2dfujiirk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ragfiijs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2otyennox.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2yzmnrgsi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jsncjgmw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lsavtuzi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2zmrcjoec.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wilmufwi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ywmfvmou.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2drdkxfcc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2effsazql.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gmlwibgs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zrqlvjdy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2llfspmpm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sgwurpam.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2excbzjhe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwmnknoc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wivshzag.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ekkucusy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2sxqrwbpp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2boecgnxl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2thyxjaxf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2aluwhora.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nxvvvzzu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2otibknkv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zadvqsji.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gudrpckr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ksukcxzz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkulwdl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2klzeitmq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ytdddvps.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvnmncwg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gribcgpm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dctcgfsc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2snfhweue.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qozfiybw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zcmimrqg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxzgrd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2esatbdpq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qvrwxers.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bxxmxruj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nlufhhqf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tikfvyot.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zmjumras.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ksevtqgz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lnfyhejp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tdeemwcd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eaeyaykl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zipxplau.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ntxrklva.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cjjdwsdu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2agioahgg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2egkdgech.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ardaghma.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kdaegytz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2walbbzhz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ngivllvs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jypjgeqx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2abbopech.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vfiofxmt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2tlipbwwr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2adqbcuer.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjuivchh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fmebnugd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ikqefykb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qqdiqbud.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lkmzfvmw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yulnrntl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2orlxyyjk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2amfkfcbv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lskduarm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hxrskbna.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yekhjirz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zeabphsj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mtnxcyup.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zcnccqfd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wnemykbv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cagmibzm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xrltzhwn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zlobbwui.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2atlogldj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wbjaghpw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bbkekndr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hpmtzyrr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2eqjphrmd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2esdyuyhj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lfvupufy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2znarbvfb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqrqdfx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2efzbocwx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcrvtmoh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xoreibti.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fbqzlott.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ombngfav.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ybaqxvet.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vzbvdfmf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2uugpbqvn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2chqinklv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xledmraa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fjfvcqth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jpiojqgz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpayradn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tjpuanzl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fyljdkkq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hiswukct.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjupwiy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yolrqkna.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2basqdckv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhcspv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jvlkjpho.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bpvdjpsx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2oixgmotj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2keszgngw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qnjutlcc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dxeucsnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rfopymzh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmtvanfi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jugsawte.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2phncuilh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2joqcswmd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2towtryys.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2alzupxwz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uvqmunrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pgssotdf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rtqtkkye.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ixtrvwog.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gnoongzl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jgpljnkv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2spbzftqh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fmtlweaf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ywscyqvy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2znwrnkss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nsymqosj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2suxexddv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nhtnfcca.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zknefwac.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2epsmamfa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dqgnduve.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vzwnafox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqeixgai.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qurtrjsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itibsyib.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqrpnqcb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lbeucprj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iihusjll.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2antkrzxh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zuqvqkrp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nibvrioi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ajuuhqho.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wknfrmig.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2frzzhgsa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2udtbgjsl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zhpwbyfq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpyjeywi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnoowagg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tqesfvyc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2daqnrkqs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fqmnsqrf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bropblak.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoeobvsk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ucqzatce.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xxispbjm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eaukozpa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2olilxdik.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bpjdvsla.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dxsseydm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hapsxnvj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jbtailpw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rwszglxy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2olmcuhin.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zaspzpbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tlxslfgt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cxgxoadn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pdvoeepo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xysvqnbv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xvuqcdnj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pqokfsty.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yglythgo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nmzzmhtn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yfmbnsut.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2arzowurg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fozvvjpy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzzplhmk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iezugech.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fmyqbnkq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rylykdjl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvmtjctw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jyzvfuoi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmgnpwuf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yjqxgahd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdlsrmtp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnsokazu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2szuwekjn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyasclsc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcclioco.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmmaeaiq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2scmollod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iyvlbxrf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gbtjdqkz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2somsoafz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pwhailid.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilctkhpo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ymtdurqj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2olccplxr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jdfnbrzd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fwukvmdi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qanazspp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbvvhbgu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tnvrmoej.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hvvyxyan.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqvwny.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lvduxubu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqthoka.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fmehzxxh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2acczypok.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nyljchbs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2okyuicgz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qrznglen.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bkqgdroe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kgpmtzdn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hoiokcvu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwvdyyak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xtsreizw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lufdlvof.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fymqusus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iobzatha.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnugozzg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzibrlxj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hzsvatll.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtslsyen.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2najdbmjp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atfkmnnc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohcoysxk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqgdbvxu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ghhcwvps.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnsjixoc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghsiqfsk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wumjukps.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kufuojgi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojaojtuh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2brbbajyo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cpfvicdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mttpnzar.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2eebxwnmi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lgkrgoti.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2akckkqjl.html


<!-- 参考信息 -->