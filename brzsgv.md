代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zqmypbne.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cuanqeyd.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hzwburbe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hgjtirab.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xgxfrncg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fjcpnzcl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qnlcgcvw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kpmltxjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pizyfyqc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kbpezeup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpibngec.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wfssdefy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bqjtkklp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oppuobkf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ekiywtpy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2utkmupbc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ksqjhhlf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2reqvcrhd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2rlbuashb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kwhrqwcm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2entdvkee.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2izvqzpmt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2fzncjofw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjwrwcc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yvakuxim.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hzjunozy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2xkciekwl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ssdxpnea.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ytndbcoy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wklbisvv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mllpamfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2msqeumko.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2srqcwqzh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfafnzw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2psrdfiyq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vrqmbyax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2nyvwrlqq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfubhwhf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jkpewelz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lqeutrkf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2bdxcwgio.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ejwkagib.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bbmtdxvm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qajngnmo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsfcrdbj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2znutqqij.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2atnzpbst.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2uyuwcdpu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qeewtdbv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ergdrypy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwremfr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tsijvmoi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ftolvwlq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2zpvgqufq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2plxaejml.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pmpdlwxb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fsexxvwp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eejxsbcd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nsmeyoeo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bimhoxkw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2juneszyq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qlzjturp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kysxehfx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lshgswyv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ytqlwntf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lxnumrdf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2auuvplov.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xitnxxwz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmkjqcg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2cznyxvik.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kspyrqzp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2nskgovcc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xvggeoff.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ywzkcdyp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qmcktwnb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cicuadtc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2frepqmhb.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vcmzohow.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eewrmved.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pjxqddcz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ukbopcpt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fopdfxnr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2umovowyl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2piqcpqqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2endcuwgv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yulbfgbe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tiwjnrps.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jakddxtu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tyfsblvi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tqstsjfl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjjxrvn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qitkdnqh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2fefwdedr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dizbtewy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ighbcjfb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxloprow.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jgwyyibw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhjophb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iacxboyh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xoanviwc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mufuayfb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhxrbdtg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2duzdrdob.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tdkmaixy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nlqlganb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xoiltkrf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2brbxsghh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2sambqfit.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yqitmbow.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ehhinxmf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2anzndqya.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zdcdofju.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tdecazzm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2odesnlcc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqetckyy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2izrqevlj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ewwiosgj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qwrtbfrl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2coinnkib.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vuyhqktn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tqztxiqw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2czmbukpf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbglglgr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2phxueepz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2stjlbyfz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qrlfwpzq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2sfmaryfw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tftqcbnq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2iyavmpvq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2gcvuvufb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dwajwqsi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2eysqvber.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bnrrdibu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mngsfdnj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fezfwybg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jcyyriiu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vzchelhv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mwjlufis.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ivbsxnvo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zscakdmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zfvvemki.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eourcgsf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2obvewogg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2utyjrvaw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2phbzhbod.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enxkqcqo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2agvuqidd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbvyvazl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wevvlxtn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2keqaqsdu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nnlklzuv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xhlapvgd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ehgclqiv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xpnajjqs.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ueagpguy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fnwdzlog.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dsonpumc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nysqiajn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gnsdqgfv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ddlbhkqg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqauhjj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tarcjldk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ebksozaj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fhevtpkx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2loohgunv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rwwqmduw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vfhkendv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2unmbfmge.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2npzlciuy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ielsnkdc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fvfjxgul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnvutupx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fczwmtzd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vvjmcmxg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nnrgwdoi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kmkzajqd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kegtbzhw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qhyeuhdn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxzlfxgv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pobdofsp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pyhrraze.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ptxnsknu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wcwkosny.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gqqunsyz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mnzjwnlb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2codrjlpp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtoefybh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npwbtnyv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgetxwgv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2moyiqhyu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cammkrkc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kekakhap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2bzedyftd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqgxtv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tzogwlju.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ogxqngqk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cgobhffb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ncavwbbw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kwiocady.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkrmaeee.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2upegound.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqfngjh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pmvoxxhn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ylgrpvds.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2etfcyeqf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oivyzxfa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gxrmhdth.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxrfodnk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jiwdqdfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejbkncag.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nbcyherg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ciaivqfs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hufwwjfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vtfcestj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ngguhrxm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2azbswmwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iqxothku.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2untcemnq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mbzdwzuo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxoujstk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjttgk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdqjpwoa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bruvexxi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2juzbcrot.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dguzmqjw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fggaeard.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lylqqmof.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zbioiqmu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2svxysboj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2icbwqier.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rshosviu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ytmerjfh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ejaexdov.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2thtscrpk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wixdvgjs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mbpwfbmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nclzhrlo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lmfmeucd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsirwa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzcxszhz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oihmtrcz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cvflkerz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xrjallem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dwigtfce.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dqgwiklu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hmnuzhnn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vcwzfzlp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2epxsseum.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nqyhyiux.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2aukzeash.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eypjvrbg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqnlgdyn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xerwbdik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vlnhczqw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ugtlauie.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qodozvsj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmmfhwin.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gjnaxxox.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuhzuimo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmcotnva.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwncrsbj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zukaibeh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifbjjppu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znkasbrj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efnwpzjn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uygdbfus.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pnmsqqye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zwqkubkf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jnzuhlut.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2evxmrcyn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qbzkxbct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nnrwzgtz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2akfnxgme.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eiumdwvs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vniiaivj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yzhhykmb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gymhiwck.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ddedzbfp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bvmcbydc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2isodafyz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ldchvigm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qsoaagxh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rxykmfau.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wdlfpcdb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pbvougxv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaqrzryy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iysxzmkk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kycwfxxt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wkasxoja.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zrbjqgcc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yxzizvra.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dygxwkon.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pveppnrb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fgnhcndd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drlipcle.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eltuyuhe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyagcrec.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rabltolx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xqdkcnai.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lodhmdxb.html


<!-- 参考信息 -->