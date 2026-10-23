代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ricagnyp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3feyxfxss.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3orftufkh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ucuihwjs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lsjikpoy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rodvlnnw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3avjigqgi.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zoftmydp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3riazucgd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyxoamrn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gxwoordn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qlinxvgc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yyqwxwyy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oxuramof.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hqprdyvd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fijuazkt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3trddpffi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xtazxart.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hslpoptx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ddvmrqac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vufpxbyp.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3henrynpe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pbjkpmje.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cknmrnyy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3nmykhchw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3auryfcwj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qmsjrksz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jywbmqww.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iojpicrz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fdbncpbq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wbxccbsg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yjqbzfie.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3dxwropmy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3dtvqoyay.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uexxttur.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3adckcsbg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wuvzaxod.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vqybrswh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3leuinhme.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3avdumhpv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sjgjxhxr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ollliucv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhihdqto.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3civnqsev.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3llrglqwa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhfxgkh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zfyytjgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qspaoevo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3onmonokb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iekvqfkl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xrrhmmja.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yxxzbibr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vofzqtat.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3mjczjxav.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3awezzhqk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ryvystug.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vtfbfzws.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pfttfwes.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ksrpzvnh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjepugl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jmqkoliz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jvvipvpc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3siulliae.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcfkpgk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3thpkqlql.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ckkjmhqj.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3amdomivs.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ntvcslkb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwyoprfp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tkupftqs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iwaqoubm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpepyvuf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3duscvvdg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jbflerul.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3fowgozpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kplnghoe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nnztywyd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjphemyn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vtxizhrx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ogpbwnjn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sxocuxux.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lkdgftwi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kgropcjn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gcvkgvxl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lykbejrt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tpwqqlmv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3anaouawm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3unulfbgk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfshoar.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkcoubkl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tczjjahz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xentsqji.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wpxbpddt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3orxcuuyh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jfdrgntf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3huqggigs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ygmaifqx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvzmscfv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zidkxuss.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vbepwbmk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nwtmppim.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjfrsuh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3imwhkdng.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqjqafhr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mnarwcdn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3oeoaixhk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkbpnedw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bixhnbgn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bwzaavyo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3froobxgc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pmubxmid.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mjthejxk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3rbdgdnms.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oeuoomwm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyhcdtmg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3raiwnfmt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjygerv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ogekzmhd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ygouzwjf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hlusofzs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ihusodkp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uvidrqii.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udhyyizq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3azlqfvsl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lyxivyti.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bkhepcyi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nyfrzuxx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sknxwxxe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fwiaiugc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kobaptul.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehkguqes.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rnjrvziw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ooodjhwv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ivwpimbv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pxzssdoc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lljknuyb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kcoiguul.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mmldeofn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dwfsmmjh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mfhwiwey.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dqjqtxvm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzbzvxkz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dzvxomfh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aamyqalz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qknvkium.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3orrkktux.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qpzmecgv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uckgrjwn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vrxbysha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yakfujhb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3erykotio.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vjivpehs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kodegcer.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3beirxwrj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iiwjiygm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mxwkldws.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kcfjiulk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jqetyoui.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hydrmzks.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uqldfkce.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ubmocfmc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yymmfoiy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3azlxxhki.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhgddstw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yuvtevag.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rmtqorum.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3sqlpevyb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ehhgsbbz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xtdgjbgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aryyttfq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdyqilvv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pefbdtvs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nrxcndsr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mugkpaix.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdsfhkdi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ltxunobz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jkxfjrzb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wryjwsub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ruhiyfzz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zvmjqznr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjfcpapu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nhbeqnzb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ruiwobzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3unvlpqrk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zopockqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3biirxsxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ewwlufmt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtaxyxvs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kuoqqved.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yffxkjlh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3enwsyjfa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hmkirdrl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qxkyzgdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylwtyrdl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xcjzxsnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbrytvon.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3roektrki.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uooyirfp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhiyjbkd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jbvdrucn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gklrwjfw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwwiezwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bjkvkgau.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgwigmzi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jsdnvfrp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yddyfbcn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ayoplsxj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsiixvi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoqucgru.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hldlwsla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxmhbvm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hrjotkfi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3frxcrbmk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ruqoeart.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3aermwfwz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsmdejn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frdosbvn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fbarijor.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3czblukdo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3obofngva.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cgcvvhos.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yvddehgh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ldjravcg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3veehmrry.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrjoqcuc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ydgxrbfb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iwsnnigb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jtjwtail.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ilbzhtdi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pykhdjpr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3epdiozfi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3skbnlbwt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3shqybeny.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nbaeqjpp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqpqdqni.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qenslvkk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juukfwjf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qmoyvzxs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hdismsgh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jergmoxd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlvxveys.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3trdpfqal.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytdedlcc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yasxwbog.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbkyvyfp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psuxdvqi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwrhpnuh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iarxgpff.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xsjtypvw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nftljpuv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3klfwmtew.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kpttptqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iwkepzkl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fsoykrim.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uxclqsee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fyiljduv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cjliymfe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wbtnegcx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cdwtebew.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikkfpgsm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdyikuod.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3yucyurzj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhgqwsuk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eqdktezm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ifsewshf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xipszlqw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3leqhrwmc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vbgkppds.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3srpvfjrl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyjtynfh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mwchbhdr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xfkzcgqo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ivkadpur.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3umlbldif.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ucegmejl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wykaqikk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yybrlvny.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rzpuiqxx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmmnkzh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytybnqwc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqkpqquo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjmofgjh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zvvwyeua.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oajieilv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gllbwwyl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emiwroup.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qznlshoz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgeundju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3edtugztp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pivtrkhw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnllhzbt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtbonns.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tprrsizs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbhndczg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kqkxrnpm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3thgqbpsb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrjivmv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lojhgmki.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wwhntjvg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bofklhvi.html


<!-- 参考信息 -->