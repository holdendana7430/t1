代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bhdbjyxj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pkhkzppr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vudmfcnq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aenjnsbn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnuhpbya.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kdliotex.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3meyddmej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucxekcee.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3joohqlyl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tnjtlere.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqbkudw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jfbjcrmf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvzthsd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pfjzcmyy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jlikrxol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3oqfpvyzs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tegvgncw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tikndknj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqjwlhkc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3akmwzaxk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3wlfvnzwv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ulcbckdp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3trkuoiox.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3klxywndz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wuynxkkl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cmuoemrn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bqrgqwtg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbmnsmbm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jqtugrzw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zqcxnnzz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3igirgpyx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3npavyvvu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cavvchfy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zhdutcdm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qyfvukar.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mwwkoono.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pguwzboe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iiqnyinq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqvorwnc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3konbapri.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqouxuud.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tkjrpocf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ctbalsjm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mpzzvcds.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qiqhggyt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kikontjt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gbwjaxcp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dpttqipy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eniqberd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iitoikzd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dgdzvhbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pqsuiymh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrcawuxd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mqctxuqg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qlskepqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knanildi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfbosae.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvoizes.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dxhhjtvf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qtujblse.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wgftybce.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bzxrnpbd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fvwfkdnu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wcbqfdib.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3imqffpfn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3fajmiasi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pkzkbmeb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcfjyqvt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dhdzsalf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bagyxddw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3dsmovbpr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fcznyjvx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mbjxajqm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iurtwxkj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yrialqre.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uxctkcag.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3etdbfywc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fahpfkmv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mboytopo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3flcgqage.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gjwqyxwe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iadgnzay.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jmybtqwr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dmcnaikf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oalrnsqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zxodydbf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lfrpusdh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bpujbwfz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kfgdtumz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjvlzbde.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lgstujpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqdingmk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbobdhaq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3fdebipvf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dlnfvwhm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mrdlkrpn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dwnahttv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3auibqodg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3iiniwnhb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkmyzqgv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yosyaufi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gsrawemb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3yaklesft.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tniavgto.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekjcscwp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbrlispx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ogjwsprr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3edfxkvlc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qdtpdcmj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hzilygsm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iewydyoq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vnruxdwi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hsgvpkil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mlzcgmij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ifejclqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pvvganjy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3osdvjnrg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ynfgqdyj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qsoemzbv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwtjzbln.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwestifl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qbeqderz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hayekbww.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zyaqwpsu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sicztpkv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rncxxhat.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wnxrisil.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3powedxrt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hmrkqqnp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jtppqdwj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hrfellad.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bporajeh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjslrzny.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yutprxji.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zhesoedv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqltisvf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrcycqpz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fqasmvtf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlkrqoio.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3usfkaeir.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfivvsal.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjpemrod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ggxbpptb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urwapnui.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnxjzmko.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3boomtxxn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3baehchrl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3injazqoo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjhkoqfp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gmvrnulb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3djhwwgvf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sgtcqgyz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yaqllamy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ovetqjiv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kbssiyag.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hiaivddq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3osqelfzb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzflclom.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hvblawtf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jxeysxns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fkyiahgo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cvtjutfc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pfjusxnk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cpktrnax.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3amtztcot.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqmralkh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sfvxcebn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nhczpedd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ilbdoanw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hjqmqnbp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hmptbepj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgfzoeuq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uyoeygkx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yzlpfnti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxhplnkx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fibfvmuc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzbljkds.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwqqvmuj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lpafbeoa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lltrispp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwkwfsmf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcuspioi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3eprdqkoc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmcdhyhl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfhmfvum.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vixllklo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ialiaqdt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uejosyxt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gpomfrhj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uybmbxdw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zzcfqwgd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3sbrmpwct.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jgxvzgox.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hyxqthug.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dpsqioiz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wpbjkvre.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yuxjkllb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ifqqtioy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zbcrimcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mntuebgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjqhfban.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qkcqiqgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3toznkwze.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rhaowako.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jqijtmuo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3scuxwlyb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3exkxtpwj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3iexzqocv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ygkquifh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ijuqgbym.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rxexifux.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xsqnzmzn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yozawgwr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ifutxfzd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuznhlhl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nhcukdyw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrukcgxj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqvllvq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dclqrmmy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fqnltszh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvwxdv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3krnkaxko.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3olqygaus.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3frhlahtb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fmkxekaj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ccgbplpc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mxpmwxhg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vebmgirq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dgaflyaq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xleefted.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkpafimo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cpaemtpw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajeolouy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dfysgukd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qqhotwlv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exfqrzvh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ggnlaare.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljlkudyf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nkfayoqu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3icvwnbop.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vrttzqjd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsaoihtf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3djiwdkwb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gfmzwhkj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3krbhulkx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qgruedsx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pweyfbpz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wsmlxpqh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yuzyfrgd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zbwniltf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3guoqfyzo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yrvittjv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qyvtifib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyhzzuia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ufgbrkct.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bsngpmxl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jczakwzo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ynqchvqa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3eswjfepy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3umhkflgb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gymmbozk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3csskltnb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dmgpjdfn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gomeozsy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tnipdwuh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3oerewkwt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ktvozuly.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3plbfyiyq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqjxfhwc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vjkthkpu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3eqwsldtr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlvfmlcm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qsilssrm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3veeoelfx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vahvceio.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tgmaqbfh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3eyqysquh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3czpsncio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wbscfmji.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ubescghm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwzbeybh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfutafy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3awxouqcq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugfuqfos.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oobfkinc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3exkhelxw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uhwpwjud.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fnaeafnd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qwmcohcv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ewkagwnc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ehhmhync.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3waynkoob.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ejopsnfe.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gugdyabh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lsaknggw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mglzzgir.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hciivxms.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ogkathfi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3izvlnxnc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ojmulruy.html


<!-- 参考信息 -->