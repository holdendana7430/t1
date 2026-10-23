代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hqomzymd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3czyfjrkf.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zhffescl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3cnavtzhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbfvyxgf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3qrtgsqly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csagezcf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nqmgxqnl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fedtqcgq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3terdjfdq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oojclior.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jxauwxnn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljbhjahy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rvxyrkkb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qncubell.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ujjlvwap.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ljcsgzya.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3msvlylum.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kvtbxhph.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3elgxugzf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3sepzcvsm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxkarziv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3iiaranyg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3gsbtivke.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jkkankbn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cmcykzey.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zhixqlcd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dltgvgvo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cdzmxdbf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gchrrvug.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kdntnais.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3disazpae.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3syfrityv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3thxrmogv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3hjgvrrkl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3uvepaebj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oawdpmxx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3bcistyto.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ouswavio.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fgeangsl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tzipapru.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3txvlwthb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vqngxkcg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ukjnczdw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vbiuuglh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ruzfbtde.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mfglusws.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ikexidyl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qrocnvlq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cinxhojy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dmufzkmj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qurqtriv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ujylbcep.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3soejasfn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hhqvmehp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ctirsnzp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3edpciabw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xqimbnar.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pnmleswf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cvfoahme.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3czblhzje.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iocbguzx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3htvmbocj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yoxyunbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qvqhiaqm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kuoiwvbi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ovqpqgrn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3cgcdoirx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rvakxctv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ekawkics.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3txvzkbbf.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mpdyrnuq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hgnbxboq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rahhtwix.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wvzmspwz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ucnctbis.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3eoewtfho.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhrogegr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3radojkcp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3flhdjfql.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnfjnyk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bxypsuvl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3grcobtay.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ywvhxhnj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nyazaejp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3humyalgh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fhfgvjnb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tnjyrssh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yyfzjcbd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3elhrzuth.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnjtzhm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pothbivo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tivovppt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jxyuscmk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rcevvphp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hsznneke.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3egjogpgg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3bqdrlvxe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uyqmjkto.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkyzjtm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkcodson.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cvqjwnms.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mqsdyysk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rjxyorgl.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3yhzfyciz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cdxzarrw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jdtfynay.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xfcidxbt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3djnpbhhn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vawnbegy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3waqfhgvg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3njcgpaky.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lodtqyfh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kztaaixj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3oodstkun.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nuaxtwwl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vvichlpx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3njskxufw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3atnuvain.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3txqqfuiu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ulmgyssf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hizjoors.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zigxogft.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxvtjlgn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lvnbwnma.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bbmxudlv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3olxbftvm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwpxqsl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqxkvwhr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bmvjxrqz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yyuxufkp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nfodsohu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mjsehekr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pbolwukp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jwzhpajd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lbttsjzz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwxkxnz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lhpxwryz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vdynsrzd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nrezazei.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3yrmcvzlk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3riyizkvi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qazuzbrm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qfujzttx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gdiposmc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3balgoijg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iglwhmhj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gxvfezlg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ebrezard.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jfzvqjbf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kqejuxpw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yinnijyn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bzowhdaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfzvhjuv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuiisxmw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chjruqwq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gwmlbvdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oxbzjvev.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mksqvkxt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3guagtdmh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rhfczekk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3csalfiyv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3advgocjr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mvkbcpzl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3orqxcink.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzuoehkk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gbvmsunr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vhvwgabx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rkyfvodg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ymcincyg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3owigwuxp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xkuuzgvu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ghgryqrj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ljyfidxx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xjhkpkqi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhqrepl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hzyighex.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3onmrvwkk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tlfvqmju.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jemgeygu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3utmkysvr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zaphvtib.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3nixitofy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpopkfbj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xohoxmxw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lxdgzfbl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omurqyay.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3kehogpsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jucvxoiu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ihaqtgfc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ksbailsq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfzoncyi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xigxjppa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qmsonfas.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ugpkweie.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3azjpejfr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lxwxevvq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rdwhjlhc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yjaftqte.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rwrhjlxo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxincxgo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eppreyqg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uodhkiba.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfbzjmvb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3auxxiyrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckjyxqza.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsxkwujw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltgxuluw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iehgntoi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ktmrkddd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkrjjzgy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fzgvhgex.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kqftqnus.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppovywwj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vbrhmtej.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adtuqwax.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xsggsivq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3trsfigfi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rnomunvv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vpjxqgjp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pquzdhgh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxcbzqlm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3otgvdhxt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxloetda.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gotevion.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tqvyvrze.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3emzldbzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jnjzzwtc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rgsyyddt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oumpeyev.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmalvzf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3scrsomea.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vbyoigjq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rrcnbvwo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vqgoaseg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxeojdzx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mfvsosyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lkfzefnk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ramsvail.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gbxumzxf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uqjcufuy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gvjgeiyq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jdrfyyuc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iahifziu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zuwwmgal.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bolfcbie.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btpcqmxo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoewossd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsqbrnir.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mboniopz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zbwhkokz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqrdixhe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euqyibjo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qwxeaxmo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcwzidwo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3siltsuvy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qldsjuvz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfevlips.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qzuksuga.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqwqowzp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzytqfgc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpxaapda.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qwmjyide.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dqrxmsdl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pvwjxmzf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mlykmrzb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dkqqckrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gbwluyqy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jqvcxjjf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tjxrvqng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nsghfpdw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3irqsbxhr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcmcmls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qutsasfq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vjbrvenq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szcdehvm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vyfjfxwr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3utehqapx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lxswgbdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sdybcndm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vjxefeij.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3teilxcfj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3imrcmzuu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ezxtvcoa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3enmvikzz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3brczhxuv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bmxwgijp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pexaedvh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3inaxyfop.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dgyrnicx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrzpwqwg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iiqlnqoa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luqimpqc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btslwdsz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fchncllh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjamquhm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ieokuzqz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3piouhqmy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mrfniveo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xettaotl.html


<!-- 参考信息 -->