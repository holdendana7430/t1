代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fzufwyjm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xnpxhggu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jrelymcs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3rxtkwbfk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uxllzqnf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3gqmneaoh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jmyjqmuc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dthumaex.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gvzriylq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ourbfukc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oaylqmir.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3qoffebff.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fjcblrai.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bkxjowva.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhioedk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dmviqmuu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwyzcnd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gxlwugeb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvdndxx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwmdnsi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wmsxozsx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3nnrchqnq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pvapaewk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tsdbegck.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jssbrcbx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hsalwufd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3honmgurc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hwqmrxfj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mzmbcaza.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbmsgtr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qjzskmmi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qoowfpce.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lxlxbmrp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3msbpufnh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kslcnhdp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3rzdovctz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qlrzuirr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rbsjtoyo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yzwaovbd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pmxmatwt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fnyaqixd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3axdfxyov.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3regynvib.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vpverkvn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xqvgmenr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rtkcnhgy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rttprwwv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tdxtxgjt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wnxvtqiu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kwnszrle.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qcrqwybo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lnqynofu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jugjhuys.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3swwgcine.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3thjiyzye.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwrfzqvq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3euoxncob.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3imvshrny.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ynikxuou.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mfmafdwf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pedbedfb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xyeiksnk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3iamdpqsb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxxlvwd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuecvwtk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3askvccer.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3smlxdhix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pfeqqitc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qxqlacgz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3puonurcn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3bbxrohtw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ruuahjxe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3yrpcctxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qxbbhwjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3irkbydxh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xjgltyxy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cjdzbvep.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mqaxtcss.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dimdumkz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nyiuyeyn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vniwnaaf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wjbajzom.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wbwlkcoo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dmdxnwsf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vcwjaane.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fqnhefqg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdnqnco.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mhyhxayx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kzyngmrw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rlhovqpg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rckhkjod.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgushxrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhufxelu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nasstsek.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3olbtwtwx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hzyxvdsl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3eaecbvdl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pkeqzbwa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jivlihew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfntppbq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xfygzugr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czknnetd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nnctzmad.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3asgjbvsd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltxmiiwn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bbvysjqc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vdxoksxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mydwemat.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yvztgkeh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ygyjsdtq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ocvwphvf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qczloffd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3miktazrd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3okvhfshy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3whlrlyrs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tuxqkyxi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bwnlpwoo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aljfgzxk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3daiywfez.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qapsqemf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhzfoxou.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pfqoitjc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsgdegru.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dlnaiyqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pyfnacqy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3babejfdd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eeuegsyj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yrulukdx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zgurwuiz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qutogtfk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3egplollp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jzqxezkh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wiscbvna.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3glzaadiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bupqaqcw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lkssflwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wdicnlcp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jcrbidaw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wumtlrle.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bixqrybu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3npskmndy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onkuqayl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nxysinwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akncuasc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qjwybuet.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3csxanwod.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3siswwhtb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yetuykuv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpkkxsmc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3floawlzi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3colcblhn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjyhuccp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkwtfflg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3muievugh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3mwllyhrv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ifmubqgo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddqyargf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbwsumxo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrphbeb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3btckbmyz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jaswzjen.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ooxmsqbn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3yqkclpgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ymmlrewn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zhzbfaea.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3skcapawh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3evtafqml.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cszqxqad.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tvgmunbi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xeqliapn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zvrejaru.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzzidcts.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yudysmkt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mssamnwz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gcqomtod.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3racgdjam.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jmntltjd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sydsyqsc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fnxicxfb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ecklpwyk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pvfgntrq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3usgfsums.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3acwjnyad.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnhissih.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yiobslbm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xnyjfbby.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3htxpazln.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxmortbk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inyyaaif.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eaxatrhe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffxopyvw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wumoyxwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onxodmgx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ksnsdudf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3goxbzmph.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tupjedqs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xiaholxx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mogqsydv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rmqmilmq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgoievg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cryioaxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yqmbquyg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kgyhgtyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fwzfkazy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mmxinfwb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jytjvots.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eilvxzwa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sdlmhjww.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3azaprwxn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nocjdqcm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3whxshwsx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jhmjvwee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ktpiphar.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wzuhlgfu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vekexowz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rbvodzaa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uyjuwage.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixlihgsw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ebimkzhy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3udfctxcc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nifmanxk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jblhlxue.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nebkkqcx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iepxwuta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nmqbksaj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ssrvjrkq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irlovytc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vggepzmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpxylonw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmvifogf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ddyizjsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3caupfywo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zksqhnuv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjyhmyfv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qqzswrvo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewestjay.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3acuvwlqn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xubptcxx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soqdeedv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahhhyizq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3iycwedog.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnuaurdo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bmpmdelu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ebyjdwge.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yqvkjjop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rrjeciek.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3whozufat.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sumrazdq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ygagsgbi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfmzge.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpoxpz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3edjzbihx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usxepfya.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wvrbrvmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blpoorve.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xzzzkojk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ctwimrgf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvsnkjib.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aowjszff.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3skklcsns.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qhpjcixx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nyreqyre.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3roacgmpz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kvzgeohd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kiqktrqu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3sldkvpzw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vqtmxsac.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dosxbvqz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrtapody.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxxvvzqb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbqdlrb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hmcgbaxm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eubtigav.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nfgbnvzu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gaxzfkpk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nnbxijje.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3saltibda.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3llkztmme.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xjcbjvwg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qizyxcgj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ixouvigi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yigbzhvk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fjegrryy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yvgvcuyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jxckpytp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmpfpjfs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrchyg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmubirl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yoruzcie.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rosuinvw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nmhzuxud.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iudbwmzn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oclubjul.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zmponunv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ilceisud.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqxdvybp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeadnfwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pdwfhpzr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3arnqqhck.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hdkzdogu.html


<!-- 参考信息 -->