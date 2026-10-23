代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3khuwtwml.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gqszhowf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ejdploqh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lunvnznm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dndhlwiq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbkzdixo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikwzhxss.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3gnktipss.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3axextbha.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tbkmmyvp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3caxhstfy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gzxfckwq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lcftienl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lesiwjax.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqrqnho.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3brjuzcvt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ljqnqzeg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lfhcjrla.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3irwozlea.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iqlfznga.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mrxkjeew.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yxhxjbaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rxayfmwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iusdkmkc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cxgvuimg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jfjyvzjz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gevfbxuf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yikxcxsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3csvubtgo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3akzwnrjm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zydgqptj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fmgxspin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xeqgijwx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3vtalofvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tzhogrkb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqeqyfh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3kilklkvp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kyowxyub.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sgmtvxol.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3yvgsmfar.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hptqxcfj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3nvgfiuvj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3klumdxig.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qglqdfft.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gtbbeolc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uwmwphdd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xqfinzse.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3wmgwtdep.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ydhqpbha.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ioerlqgp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjrfawu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vubjesde.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ydpglvsg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pabduavx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jtqkoyzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ytjezyza.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fpamhnqv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3zrrlrfnq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3amjjckcf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3azlpmbzo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cbrhculw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ntnkmatm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lqldjhcc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xzempgsn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lrrtdfzg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ncypxpjk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bdgocxjb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvhdinuo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3liafiqve.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3igxubpdx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3inwqtctu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jbnkgsvw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pvfjuodq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zxqjhzgs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3elqqxllh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wfzpmgca.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3coprccyt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vpnzxgsx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gbeeudqf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovehfivc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3acijetwk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ygxwnmfd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tnbvyjrb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3irtassra.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dsclnhql.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mdqvvqlp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fmohtzau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jqfdpvef.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sortjeme.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3sukjujcc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qswjzdsg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hhvlnpgs.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lqabxshp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jruyluzx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pmerfqgq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3luiwfoqc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3euqhazci.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wcmzmrvo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wltkbmog.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kgzhlrcp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qiqkctqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irfzexsw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kvmrfybk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czhejkva.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gubrgvqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fbotyohj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3urihfcdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wefigaar.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dpeojwme.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bidddgxz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wuymfjbn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cshlzvtu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hbsblang.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmwiyxzm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3nfbcfqym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3goqwmimi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kcyxqmxi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yismrfxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3abuffakm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3phkqopab.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3euoslbel.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3swbrklon.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ivppezpx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iszzefft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iesseafr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zqtpvtnw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cngxmvic.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rptsdutv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cowzyjqo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jhamlidi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jjjqkvej.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hllgkhuk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mfhtpqmo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pmynqxba.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uvajbstg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bwdszdfp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xipltimv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ggmfwmjd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fltxrira.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3plxhlnyh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cwcvqxfd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wtviputv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntkpcvos.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djdrioyd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvvmhqux.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3irlebcbt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ndfptept.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gladmlpt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysaksxxw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wpzumann.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bycubuwu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kbkqttgt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpsgvddd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgcklbo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jiuxgrho.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmslzoum.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmjeorfb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpqwgbrx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3biepethv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tixvvrkg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vsomhnsj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wliunigk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3izuqnxwk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjbetkjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jhajejcb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jvmnfkeg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yfiqdjgd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uiudzccz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdnqdrc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncqmrrdg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iuyvwoqg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqzsnm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dwrcggmm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uednuwvq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xzsvvihv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wfpebqky.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xczszqry.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjjskped.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rsqqvcsu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tdabsvvo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3scybhcqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gnybijay.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jrmurawm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqctpblo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3plcnrrxb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gwqrveni.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulpieosi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwgegdia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpyxcvvx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voatejvb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dboxvvfv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khnjkqga.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwkiejjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywiczqpm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlrgvosw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqdtafwp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3amikkvxu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhnvlqtt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bymbeylw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxavthne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3laxtocen.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imrfxpmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yzbbcagx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xnfdfpzb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kwleejln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ziqvefqm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fhhlauav.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dyitaxnc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bfxjmoxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gdhspile.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lsnlsemt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ohtflfbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhpofvrv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3muzwcgyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfeweljh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3klljztnm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xltoofmn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3corkfpek.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ucuseydi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kjrjkile.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvawleqj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xmkkrmzl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vmkttibb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdtvpvva.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rrmkptnk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jmdudsmc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilqgctgj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3edltrdvc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvayvaew.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3acgderev.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yynslwqs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zzlcwytc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jwnqtvig.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gzdwkyki.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3avkyuiuo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gkykifou.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qrgzjezm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bcdfscct.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wyqyvgoo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ojhhvyok.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3igmqqlhr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nowjoauq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cdkwfjol.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vxnvtidv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wicwklfh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fnhdbslr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxigbpb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lgazxwbn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpnxxzp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqktsrkr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rmntkanb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3svntlcti.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3olzdohza.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vijakkkn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsjrzgpl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckqpiqtz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lkjjwexf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ctabrveb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qciseflc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnxmsvfv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hduufsfz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cquupvii.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxjcczr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ctsrvyqv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpblefwv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnfkwffa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gzetvslm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cgweavum.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xbaaewdz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ehulmszc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kicghtqv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ejcnqver.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mapjmabl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kdsykpvo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fpnouvau.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3avbevyzo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fxrfwsdu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bfuipoyn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dyjeqsbd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ohdxcoai.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzgvhpjm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rptondfa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3csezebpj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xemsqqed.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yawwzgul.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qodqvcjz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgbawkeh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gbjymgvq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ntcpnnil.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rolbobyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ayuncchm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qlxgnfly.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ufbskugq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dphsblab.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dszvvvjz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mneuhagu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3apycwdpx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xkmubvwc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mtytabsv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hbfcrtas.html


<!-- 参考信息 -->