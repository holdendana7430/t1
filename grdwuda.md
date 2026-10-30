代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gebcettey.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gfvjhzxhj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gnnyskfjh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/ghtcpetqm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gpahsmeor.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/ggpgrltpv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gjjxgjozd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ggffadqhs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gggbtmggd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gznxqotxv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gtvaxdgat.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/geaqjgjpb.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtpegoirx.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/grqxlmulb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ghdnzcinp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gwlgorkta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gkovkdpei.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkqwhsvpm.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gzoxhdntq.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gkceafpup.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gkszrkbdy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmmgpyqsj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gkariozzb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gktvcydzq.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/ghupdoojf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gaswxetkh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gdybjwnqm.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/guzemqung.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/ggoodgnht.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/grqgfhygg.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gfgsqjvsy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gfejbhssi.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ghorbllkp.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gwlcokxej.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gwisyvmhm.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gyyqzdpff.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gsusmjnia.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gxdgsebwy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtqgmpbnu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtmslclln.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gmvwmdflk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gqmxawyau.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gryokfccm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqrlflfcj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gzceaxyej.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gxcxtqrbs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/ghjdkiuys.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gbuawkbts.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gwqkfgevn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gypudrvtw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gvwaacjzv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gcxtqyftq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gbtsdnggy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gjaixpxbc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gqemyelak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gngjltack.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gjgoszfnj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gkdvbrzry.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gdyquktui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gibeuvebb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/goobxccll.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gjqiiephj.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gqupzcfvc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gexjqzazq.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gxjgvylui.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gmorwjtkl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gdvesvxyx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gbyehjhpw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gyspdjwcr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gbgqelbfm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gavhhpalw.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gzxcgfvpz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzweamgfg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gkqckrdpf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gcfwrmvpc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gdeceyach.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gypxiorua.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gmczgfiec.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqjalbeqp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gdwjduoft.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gspshyfdu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gszlehhtm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gekrbvenn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnxyfwvel.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gekhvyfyw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gpoxvhwsx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gkkgpusfp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gslizsdnd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ggfgwyjiz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gaxlwvpql.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gqdinicqc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghfwdbzcp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ggsyozyjd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gbshgltzk.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gjewwjmiv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsuwtwcmb.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gmxpuhmdi.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gwekscsib.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gkfffxibe.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gakvfmrhg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gaajqmvue.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gwpedlpln.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gshyyuwpt.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gmcwvufpo.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gfrtwgvoo.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gqbiusxyu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gsnwwzkdq.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gqkwjqbvg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gigrbpegk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggsskxxgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwehqwdxq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggagfiuru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsjbnapob.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/grqffhxcc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtctfepep.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gganevyxv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/guctawssk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gwqcctpke.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ggvlpbcky.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjiwipqdh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gobcreaqs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gbgjjdjkp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gjkyxuaqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gytatdwez.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqlytikmb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmadejqqx.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gydsowpiq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gedwvzsei.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gooqanree.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/ghgufnvac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghdbvhjph.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gfmpwwoik.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzgailxrh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gztngdwgt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gqfyzyzsr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggmqmpycb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxkfpgpes.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/ggwmybksf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gyomerppe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gyandwojq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/guyhlqevu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpgksykdw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/geuxmqynj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gajebpvoh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/ggopisnox.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gshnfuwsg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gticavclg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gbnwnyaxq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gvkalhoop.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggoformwm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfddtfbft.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gpmxpifjj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gwkkgeebt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gmkucmnuy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/garssjhap.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gblujzshd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gwhpjhwnq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gpxzcwnhc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gnijfrsay.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdfryvzxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gntxrwfdv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ghqcbgcvj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gjtbbcuno.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gpxwbeabc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gmricbzhd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gyjjbdkpt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqyiqqemo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghcobbdlt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gknpwynag.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glnftzpcc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/glbrznjww.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyaqoejmk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnkruwsel.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gyxpnkfdx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gejdqdykr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkhxcbuqv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gungmsdhl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gntlzubsp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxtmnygvx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsltylkmq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/goxalyjmt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtspkvcte.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gryqpytie.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/goqbpkfsg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/glxxzdpih.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gilfnfhnv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/garytrbsw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gvikobgqy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gewzpohsz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/geefxnbgz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gkclatngm.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gcdnjirus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gpvjxupgc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gyjtvzxvv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxkpdnhk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gxngruhmm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gamawluzd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/giecjsvjw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gghahvygj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfnyoxwxo.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gkaudumrp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guhweukrh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggzyvlhsf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/goslnletw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/glsgsyoet.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gcbltzcxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gjvaollsj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbjllqlvx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/grnmqcxdm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gyiuwaslj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glmvvvzqi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gljjmrfzr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/guklxddmo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gecgezaym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gzuoxpsad.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glzwwiyes.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsemdxezf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grraodnoa.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gchirrkxu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gscdarekb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxusurkcb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gzvpomimr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmdeboqbl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmohocuhy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gbbvtnbxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggnbeweng.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gvfwyosae.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gesiyuhql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ggytjjgbu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gszasopzt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gaupomghe.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gydstlusd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gwtnboqgf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gflpomoha.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gxybsjyte.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gevztyrul.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnnrpztem.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gfyupbnle.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjukbuazt.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gcbplqgph.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gckxzyxnh.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvjyudobb.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gosfuyflr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gburuiypa.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/glpudiltr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gstikhqbg.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gzagvcxzd.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/geupfkkab.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ggpyoxueb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gcffgqpsv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/ghmcxirub.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gzuecneop.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gcmshnwrr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goptoodwi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gftnbryva.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggujcmugo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gvuowrbjd.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gschstuta.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gxwqwpair.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpcehpxcc.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvzxpvhli.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gxqscbidr.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gdonfxjuy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gbkutxwut.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gelgxcmju.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gticonmgx.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gwpimdqzs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gpjuatbks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gwawytsyg.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggyhcjaje.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/geehaiubo.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvztprwts.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjfiwvbsx.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ggblkrtqj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gywydtzyy.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gubwxejst.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gtefbqjmx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjtugkgsc.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gugmxiohq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdjigcobs.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guyhfxcfm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gpkzdonkn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gzyzsilav.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gvwusdpwe.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gsydfcujs.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gzorhxxeb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/grsekllkj.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwjjlulez.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gorpyulwp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gczwerzkh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/garxthtng.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/glbpatjnh.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/glxmhwddi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gwrselpfm.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gijagqzoy.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/goiqnsfod.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gxxcyjtvp.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/girnbanmc.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gsmzppnnl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gronecqaw.sHtML


<!-- 参考信息 -->