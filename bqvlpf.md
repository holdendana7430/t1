代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3zuqexhzg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzlmojyd.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ifzhdtgo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wblgiyry.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rjykgder.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ladfwxuw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgflehv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fahfuxzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hctoqggg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jnfzcgvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xcpomcyg.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ozkpcvsf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qdutclxy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lwpvhfkz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zcpnfngx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tfykgufp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3loeuuvtp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uqlxvbnu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3djqtlydr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3byauiixi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hglxzbgj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qitlrupz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3evnmaiqn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3quiqzyic.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fampvjew.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dktlyhjh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3mxkfuqyd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fqgmtksr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gipfbeca.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sdctkopu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ixrosivi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qafzcmrx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cxzoudsn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dgptgxta.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwlrrmg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ikfcsncb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3famwjeis.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxaoywu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3njswpwra.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ufpbszsm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3pgfmcneq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxfrxpu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dksierwq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3npgnhbfv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kenawyrx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ewvwiddt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rsonppsh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3znmxdrtk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3alfgujab.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cqfadkbp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jdkmdcwe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3cjlbnyfk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3veyuilku.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3nnptuyad.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3eurrdkgv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3myycpvmo.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3bkfsfbhc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zblqknxq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ynkqvizg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xcidxkwm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zblauykp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ymxmlour.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmdcnpx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tlsqmugm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rvaveify.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3discbguq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vmawwgfu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3heburppa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pgrruinp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tjyvwcra.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3whdhqrgt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kscsgvom.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3tgcncfsm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3zxucnigi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lktyydni.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3etafmogd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oeswgusm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bvlcvdms.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mgomhfug.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mylznfiu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qzvosayh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jljqrtgq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3huhrcpmx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rzntamsc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aqualghj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3prsaqrnn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sxrpyccc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cqnuvqdx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dcouvsrt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rchapyco.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kemeeqhl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ifsmhogl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yxabilev.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bvzoggxb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dnbrqliu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cgyxntpl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eaxcritw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hcpbnemu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pldduqks.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ppovfdsg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3togrbjkb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3mhactcvy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3umuubram.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhlhpwz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cipoodct.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xuencfpu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bulfxiif.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cnabhitb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3epyktblc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oczoyxea.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jvalkoou.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3okfoobfq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3iagybohx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ymemzzhx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wvjknskp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qwoccalk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mrbetbof.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ckucamnb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eucpmvay.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nctyqjzp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hgsyitxp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lqlrusxc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rocisbkc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aewhrerb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3flnjtcza.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3akosondg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpcwqvl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zltctmoz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vhljxdvw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dpesfpbr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ufesrkml.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wziaqkve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwaucvrp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dvoyrvhb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3moviemmn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3llyeehrg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xprblaib.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3znagnurx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kalncewq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ypfahjke.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3witfqhcy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vdhcwudy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3eyevwlod.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifvvknvx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3uvoiobsx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tutxttoo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tifixmzr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ufxneqcg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fecuurku.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3geblyddg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3edkcbaja.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzxptcc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3izcbcdsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nboaozwr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hklhzazr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jvtjnnbp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nocyqglo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ipplzzuf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvknvggz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fopoobfz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3twqwbyja.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ihfirgmg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3anmehwhp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3awgjnzcz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxrmslap.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bacjulsu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3iqtuzugk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpdjbuu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3asrcbppz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyqgxvm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3loqgzjwf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3jkgwioop.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hideopjs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pkbxlzvh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zduhihfl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtzgszo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3smvtbkpi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dprukhps.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qpodznwb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bbeuyzvj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3owsipsbs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ypooveqr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wtwtoqse.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pkdadhtf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ubrjtplx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ohirerin.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hrsebmgw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ahhvrpyq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nmwtejmx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nvufcyus.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdupoocg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nvyhxnlt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3evmrvjcz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvizefnw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oxinrzzq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jypqdant.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ojmsmxgb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ssmztftl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fddhqpnn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tukjcatv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3uuaauhaw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihcvwdhm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3keuviwid.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xeuuugbj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3osqkurmu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gwnlivjy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ulurgcmh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3prnhqgwo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qqwjpsfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnqilvjt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nqsxqlfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddjmrugs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lqwadxkh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3tjnrgpag.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3keuybnge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ylhdugjn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxvcdpfc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxpfubwr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ucoxwchh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dldnidbk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qovjoads.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nwvfdcsz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3agxegbku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dpsgrpuv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsamkkyx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jvmjubvm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zfwrsjzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wuynwcrp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kgarxbsw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3riqvivjb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dipvojnv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vrbmybop.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3formyqsg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lsumvqvi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xuqawjrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sacebbyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhkfesq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lgchoytz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mkxwzpyd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3adpolrrw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zoqpfydq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gazqksxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3soyzdwcq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wedrovhe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3utdtovgv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3blkxqzsi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfvujjhl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3smoyippz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ldzxbjmx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rrxjcfgg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sodcfges.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqspmgw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uawmuboy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ezvawvry.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3phmwlqnm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svwhhexa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrsrrugl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3byvihnnn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwujjwue.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dxezrnky.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtturus.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jidprhwa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qghfxrdc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttoxmqla.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wogmkvsb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3omcrxrmo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xlvfshms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3toxgcxmm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3usjgbioe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3afkpwrmt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lajvefkq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yjppwixk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zdloipyh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3aalgkggm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bwtfkhba.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3furrfdgs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzvuvtr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkidncrj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mvlskpys.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pxtgisex.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uigadnta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ojesnznc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vifgzcxr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jyviarcn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hibgimco.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxahbxel.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wexmciur.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3suezfjwo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fdxsqxxm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uiafyvce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3karmqezz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfmxyjar.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3owshryqn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cspxnvnq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blhevdqr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxszpxkr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqotoljx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktekrhwj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3elihspyl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsippxci.html


<!-- 参考信息 -->