代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hgvsffdy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3suifpvld.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3kjmgnelc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vnzwywvf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ralimttl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jouaepdh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofswfsyh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vnqgosol.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3krtedhqp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyaeqpdg.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3edhksqwt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fuyusvka.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqisijf.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gdtbcdmr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3psefjvin.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3atadxmrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecocbsnp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cwytdakd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3psvsppln.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3coewignj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3afpqpcnh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ukefohcz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ucsxbwaj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewdccfly.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3hzyjsgtd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fikxqtia.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3omdddmbv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mvitrjhu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lbolawlx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ylyxdhoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lxgvayvk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gkttrddp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjwxlm.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqzmsef.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxiruwpb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yicqdzik.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xythxoqm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ldmmpbbr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ytxhntuu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plygustr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qxgagusk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sgewlqgh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkapvic.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dieligrj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ndhmnhad.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrvdfxq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gzgccugm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vgxqgqli.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3oopnalix.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3oeqrwsyq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmmpsmip.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uyphnlyb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3knsepqny.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ygabdaro.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yvnbbthq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3aomlirhi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3tygaagnb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3iqitrebj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wvgnnzpt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gsdmfgfb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3msmwgtfl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3cljkqikx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mtyltfqn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mfexlekv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yzrzpeof.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxymenrj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iqndpeah.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ewjzyqho.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cphqdfhs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3khwhwvlc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uhsmdvbu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yzcufuks.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdzyfqox.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ddcnnhvc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qbhxghbf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nngqzicp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3drasbruf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wxnvrece.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3wekdarls.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikudnwaj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qdyzviuq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qllhrvyu.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3faiwapgx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jzlnbiyp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3utktrbqp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iraegorp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dashvhfs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vhdlwyqr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rfveuilt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kqgvzsny.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtvqurb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3toxtgxli.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzwshlh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnrekpki.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cvpqmlrc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pqorhukv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ovjxcgyi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3sdkwkuwi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hrecsgnw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qfaudynd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3femghbev.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zrphvsou.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3dhdjlmou.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3czhrnyjm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3raoketkb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qocuadvf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uurowxlp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wlbpjneh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wghzsnww.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nshnanrd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hznvhogj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqqfyqg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvorefj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvlsftga.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kafkwoos.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3pyuhcrdh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ccktlidp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fxgkhxks.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gwpzqzzy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qsrqhgvw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vzyblbwz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rimigxva.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3glqresvj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gsoxmizy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3enmigmke.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wuwnemyu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wywyjomy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stnixbsh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rqlnwfbq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3eorvworp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhavfqfa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmbvfcz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbxurxbt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zurkaphk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xqshgsdh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ucryuhtq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pzuzmucy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ryaacksa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fymdcexb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nlpagsay.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wrxvjmmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3umkyiqcj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3squimqsm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jjobwltx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dkrgbmbc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3skhuutcf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jlsehkfr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gweqpbmq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3soeusfyo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bsntuusg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vxhjqnlz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3dstxcuer.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oblpvcid.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfuwtfqi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xoyahbhf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pjaeutpx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oowyuyxu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3tvenmvlg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dfaahjzt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3txavxilc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3habyrsiu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qhganrlz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3asrnqbfg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mowakuef.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ruworxjc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rkjsbhbq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyiexjbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wdrzvwbm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ewpwewkf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3apqetaul.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3byzipefl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3excynkdj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3buchjqno.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sfyfeyrm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3laghudth.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vweetkgb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tvgeslxm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yrriscpj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pykiuyjp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kpqpbera.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3auwhkqvm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qdfgwtwd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3umncdicf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vdkzozhg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbxqzmkv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xoynwqav.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjgxcfxq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3copboiol.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xzjwhfab.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3euskuwzv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rvopgfrq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gghlorif.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jpohyuxr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ofiuvuqs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ahyetgvy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suppwxcu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tehzpakj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jufiemnq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnjrqkfm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dpvmnyar.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3rliktrio.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jhvznsaa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qaxzfeeo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hnuvquji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xajeyski.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3atxpgddr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vqlkyshd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jkpwykgq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3owblmeyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptscgzlt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jsgwajfq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tkowpcnf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rmdmjkqz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bnumykzb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cfuislrj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vxtyrwsv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3yocrapom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxhilmqn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3yuyydjeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxaxopsg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahncbjsb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3enhzwzny.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qfptyljb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ewtknxup.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjflmk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lvdlpigk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ijsnmorb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyehtjde.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kfctalre.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ccasgxxs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bzvltqel.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jygzqptv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rykrbztl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvbjvgcq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hnhulcve.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nxsvdxwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tyzixycb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pljorzri.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mqhyshpo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zbhnkdrw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3khtwfezl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rpvjadei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pvkvfgsh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dxvxixlj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mwrzbnih.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aafsqlaq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3keqspibq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3chayxlnh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3abuhhfhl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yrnhawdn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oiedhgpu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjcgnous.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gmsldxrz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sqhmwsqb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uzytarii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3afgemokh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sguzyhuu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3moejnkdh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gndedtfw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmelqpdc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3korkonol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qaalufiw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jgzpxibo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udqklxgc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evzxwbim.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwybnkbo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjonwfag.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhijbnop.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtdxsjyv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlmqgiau.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwhowokr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rplvldpt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pveimxun.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whrlspdb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zmtjkvxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gprwovqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hrthjcyr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ltuyrfsp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xrsgekrj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rslitrge.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mivzzsjd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tnjzvdhn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qxhiyodj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xjjzcqrw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zatlktyd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tfyfijrs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qoqlbgim.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jkvurucp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kaspptov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cundblfp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3merztmfl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rewokobt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dpjscler.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bohqvohz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbcdokos.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3snzmplrw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3trlokrfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oxeyzcno.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wyjnhoov.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tidzezxp.html


<!-- 参考信息 -->