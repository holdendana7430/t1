代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmegaagij.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggefbhqbf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxciqqgvx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gncebisud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gvpevjztv.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gpxvujsio.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/goeeomdjf.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/ghsqastjj.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gjdaatdno.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwuefvets.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gvhvgcbrt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gmqjwvsjv.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gbeghcmmg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdfysae.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gyrypobpt.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/glwgoymld.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/givinxhkp.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gvbtuplmo.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyunidoxu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gkqyixkna.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gftoljfjq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guhyqumot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gjyrammdn.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gxobupfne.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gyvmgmasq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gyzmaupov.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gxwhgtwoe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gibkixbkd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmnxrkfni.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/groqvvyne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ggwdawvdj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdcxwmtxm.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/ghqmcoghf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gtshhhpie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gpelahexn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gbpxvsbpt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gffbwmhfp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gpigulsfc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gcscjhotw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gxlgqpixd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gvzyrmgvq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gsanzaoqo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gmqetjsra.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gnzarinta.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gzornjhfl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gicjqvzyv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gwagnjlnt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/geuhrnhwm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gzoxofqdk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gicwaevel.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gppigngll.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gzprspblu.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/garsonhxe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/guiqkinjw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzbmapir.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gmlvfllwj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gacajqvkh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gphkqgmcs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gkuluxgpi.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gtjygvhxa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gtbqqnjly.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggmwheiir.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gnnfuuyyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/giuvrldic.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gdicqedxu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gkwjlayey.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gewmvtjnl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/glboqswwb.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gqkmotxxx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gjfmjxixn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gwgvwgcpa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfmdwvohy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gcvjnscob.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnkycmugu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzfzkmtor.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gqajehyvs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gobtmodlq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gffnksrok.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gkonfilrw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/giarydqkv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/garyeitjw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gokbrhwtn.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gindnarki.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gxhjrsimj.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gzwyruwoy.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/ggihzyffc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gvgwnlvez.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gwlfjishz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gizckdlea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gsufxouzi.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gydvddjco.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gdzoenvoj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gnsrjbfrc.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/giytozjdl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gocycaixr.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gagvkdiza.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gnaevwxtr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gbvusedqa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gheeuscei.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjbfhuzpn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gimvwwtjf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/geivflmmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpbknkkjo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqofjqdbv.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gtpwlxzln.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gloewhfyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnutwcjiy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gqrtmnsgk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gkfvcsqrv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gsyizwrys.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gfacbtvuw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gzdwdwndj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gonugiooe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggvrgpjou.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gbxgwlqic.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapiuaevf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzozmaqej.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gllgnnucj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdkxvijht.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gdkvtbpbq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpzuyqwux.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdqponzix.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gphlmbnjh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giucmxisi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggsdglpen.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gjcjwarck.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gxogqcrve.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gfdecrgsl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gccrrtzqo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gozwuabil.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gbzjdhilj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/guzerfdpd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gzucnmzoy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbnxrtrfr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/guaxpituz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gratcltdx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gjjbvmkrv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/grkrupjol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gauebpfnr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gzshqdsra.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gmeeunymn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gkkcytuzo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/glstdvgmr.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gdqpbpkev.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkxpdlayd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gsbvlpvfs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/grqndqwks.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gqtozrgsa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/giznekfhf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gtwgaquqz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gcnbdbbuc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gxecqdhzd.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gqlhktcjg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gjzkrwvcs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtzfhwbvi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpttrjcrn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghkjasbhp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsloaewvp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpfgwmvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnosuxoya.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxtqfhzad.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gsqqeqqfl.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdsmywbxl.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfernlsaq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvjyzmmek.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdzavpang.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/guynpvsoo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnlsscrhm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwtbcydwn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwlommocg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gzdxwjauo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gjscvggts.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/ghwazhhts.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gykiqfkdt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gdjtwiyaw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gkrgdqokt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gccfiwgwk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gzkldqkdc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gehnknnol.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gjcfqdzpv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gupsonxen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gagbaiwaz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/grktyskxv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gvlumwfgw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gtnhitola.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gotwewzmi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gqvbxmexc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gpquycfhp.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gpzluiemf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqljwrep.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggacendve.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gegpuxykt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gjwgdgwid.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gglbuvzot.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/glwsnrsul.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsznztlkf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gvblujknq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/ggvnpwidn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geyiptrfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/geaivoffq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpclbcsfd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmvamyfso.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gmidxqxvr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/girzlfecy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdodeuuqm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbnjlxapb.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gqqogvlfd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfrwvjbne.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gxygpqsyt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnytrydqd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gsvewmwbk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghbhzdehs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gtibqwttn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtklywemm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/ghsypxuki.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gmbfrdldi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gfvogbmvn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gxrgcsttb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gxplwfohb.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gddbnfome.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gzhiqkawu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gtxbomdfa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gmitwhnxf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gmlujxuic.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxgwsitny.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gfyqvjpcn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gueuehwui.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gkeitskhh.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/ggcfmfhzl.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gnmhmhqgy.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grcgayeft.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gxffkndou.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gmbvbvfpx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/grixsacby.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gjbsfqouv.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggohpdtxf.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gasepytou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gxdtcijip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/grouqurlf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbguqjzvt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/grglfflma.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gquzkztoz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gjinitfay.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gnkapznse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggnecpshb.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gxtycyryn.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gyglfwfvo.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gbbeybxri.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/guivmyloy.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gycixpvye.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gixsvivwo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/guldfpdbw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/ghvnmvfus.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gozhrxgft.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/ggdewczpf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gzqawyudi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grgtoegec.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvuwibgwy.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzkifzxlm.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gigcbwhex.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ghsdnskny.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ghbfgudai.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gapgmhddo.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gxqlobxvj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gdkbapytv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnujuomkg.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqkqfjcpx.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/geijmzysl.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpfplcujb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gvypcwzed.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/guwkbkzzc.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gptuygmlc.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/ghvgsdcdx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqbwfrkmw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjrtptwim.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghxomomzg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwehjepg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwcuaairt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/grhkkqhev.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gdgfvhcgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gdyfiezmj.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gvcnbgitg.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gyuhwbqvw.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gjgiraozw.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnejvjijy.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/grkjygauq.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzgzxdrku.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gprmemzuw.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gvhwdfpbq.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gebdgvbqj.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/getqsclby.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gekvqminh.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gkgsicmei.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkukcpel.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/ggaidqbaj.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gozgbbvap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gaqntiadm.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gxvhoorwo.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gfyycrvpg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gltzfdrgf.sHtML


<!-- 参考信息 -->