代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dhsmwlbn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mwkfqtrx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tagjdmdv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbeudcqt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3swnezxui.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3kkirrzwp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zwnxqwhd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wrdhdewg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3nbzdenav.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3esgfcpnx.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sqqihskd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmbgvdj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ououstrg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijdcgzmy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgenygev.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hfooaumk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gzaqykjs.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dioxvgba.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xevlpano.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3boeocqmh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmrokdbx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcloxsj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sejwubzu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jkukvdhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3hfsfybbr.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wrrsnuad.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pasahxqf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zhbmgstg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ftjzmoxi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3mexuquvf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jhomuxke.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xwitblmj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wfpdnfoj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mpgyoghu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mrypfxfa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3snltwxri.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rhnocqhp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3oclhiiib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fvozdbvn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qnmslkcx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3csyvkcvv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3rltpwumh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wvmcffiv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vljgqbjs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3djpqpise.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wihbtwtw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mktjyxhr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uwhyevki.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3whsfqfuk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pwllyhzn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjvrkzza.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jnhhkdoo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3woabgbow.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3bggxvakh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3edgdmows.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbwqjrcp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wlcnxnxr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wbsfivyh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jpmyanlk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udpgsoja.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3sibjktka.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wvjsxnju.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tmpyvspi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnoxvhy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3szedjphd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzdeuwf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ofybkith.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ygajdyrc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lzkjkioi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fgsvlues.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xcjyvabn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3unupqhny.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3avaxvxyn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgtirdx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fxyczvjf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mxzodyxd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oaecanzc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jruxmxyp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3idnbjdlk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkwixcsc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ivnrpqdo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bqltiwkj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hrptuqca.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3crvlfytl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzgjmbz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ssphehww.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bgdkepnu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ypwfyzdy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qvsddzob.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oovgtxsj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dcfheuqh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfminfsk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ztqmwige.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zvrcrusc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uzkiwnsu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3muuytgfq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ecsgajee.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bdwobebk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hhmwrblx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vhathwhs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xhgcqkpz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kipamkoa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yfiofdpd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3chcrnpbx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zgpluxqc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yokefuvx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ncaghjvr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wrlgxlmj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3quswnyvr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jjbkdrij.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3trrsrkys.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3umcvcodn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3endswzbf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qdbxinno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3earhcdjy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3crowzsiz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lxhdkzlx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3otxzussu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3unpgpuie.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vglwbefg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gvjgvzsv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mxidwjcc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3osuozpcf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xcrctcfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mxlnjqpz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wiolohmv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bpkjamtv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ddtegrlm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcifdnrw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gmcngava.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yyprntqy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvcylbxr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3irntywut.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ztkuizcj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vrvvjbud.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vywukkyt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3runclrmm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3purxnjig.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vphcnsgf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iqodcxdf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ndjplrrm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jbnmqsxb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3icnkgubm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qrreczib.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lbsuanpd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3idlzyfth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cexvffja.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3alahjvnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hljwbflq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bjimetdi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mhiepcmw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fybwczph.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3disytklt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tylztrav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fkbooyzx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fesqmtfn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ppdylshj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwsgcuv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tnhfhisr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bpbzkoyh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3glfbszap.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vjxjlzfr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3irgtcnhs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sfcskorw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kaorungx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gdqnfonk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xohwelka.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czgelhpt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3eialtoav.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jzyuvqys.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xbxabtfo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3grwgyjqd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dlpriiyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rptcsgri.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3glpaskkj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gbicgnfa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yeaffziu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fuuimwxz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fvzokglw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dbzmzytv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dqmlbfew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zxhcpiws.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mbgkpaus.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hguekvex.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bnibpagc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rfhpsbbv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gkbmtgbi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jpdcrkij.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3appbefdl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vvocmryz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lcyogenc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qwoszyge.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3egceszod.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3oktivons.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3etrzghix.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikvihmlu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3biiymnzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icmxlqyu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3erktwigs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svgtlfmu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wkhkiqcz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jyqeryai.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxefqzjt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pwebfdhv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ggohyosv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sqmdlfvs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jsgqwtnt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqjiucpq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eviqbudn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wnfnwxsh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3evckncof.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3majahgzo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bbnesvqu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikgtlsvl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qoonuaxk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vooaryfr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vydadqsq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ginzzwtr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gcdsjtbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3oaqqgsia.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ywnidszs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfzzpxz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zzcshyvt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iqcciglq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gfljzsim.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nhoijskc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fqdhedkm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nkjqvhbg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hffqpgaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ssipoptz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wxdspick.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kyxmqtgk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lqyimxyo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gqaamnfe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cpufuqzc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cohjgzlw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nyrofeae.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jiyaxarg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oznhloay.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaobqjyd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qamxlqnj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lwhlhvdu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uisacqbj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsmrzoqu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjplbpgk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nolaidvb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxvslvar.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ceuakesc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wncvjleq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3excaibcw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mocjadkd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqfotbxw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcbyahfj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wkbypmhw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wkhygvcn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3siakrxfd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kevygnqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3viqtbevo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wjerbxyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qqchekhi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjmyyqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3eyaimbpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ojrdfqqz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3grhtdoda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdcojcr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jmyuuvtn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cnfkeqai.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mfprdhps.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hugoajpd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pvuosmwu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oqmmvzke.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nhmzdfkm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ugcktpfb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtmxvaon.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdkdrfyh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jsxfddgw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nwgvwthy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iohukcoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fqvngyko.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwzukyfp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3udornkgo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qwblpfaf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrtapwz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ifasjtrx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmokqyes.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwhdsprr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ryoyzczo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oapemfoo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smzxppqv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3panprsdt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wfabylvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mougwtxz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mdltjbuw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycqysptp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yocssdyp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lrfzctum.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yegyqblt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3unevrbje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3anfiraja.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dastyctk.html


<!-- 参考信息 -->