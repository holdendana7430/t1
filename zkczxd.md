代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ofdjsgaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xzbrtkgz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkxjdap.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3covgzson.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jksvgbcf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpiyrcl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3etlwhsjb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kklobqav.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vloihqfm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bgyuqrts.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdivqibj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hksqfuuj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpryxf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gomqcqnx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pwavfqzv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrovdfew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mfdtfqse.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ydodoreb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zruelvrl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ujthnthm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eeucgvkj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mlzxrupj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tixpmiel.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iaejuwxq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sstucvmh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3waaebkmb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bqximxan.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jkheixvr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3trhygefl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ibooqgvf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tfwrmpmw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccixnqzs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjwfdqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3upliqeta.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bkvuhvkq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xkdfgkgs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rdqhkmfj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kjkqnlka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jrgbgegk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjnfdwh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ilxqtbmb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ochyzmay.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcslnsi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykuddsbo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3knwsvpfu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qibkvlbw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sksdgyis.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iplujvgk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuujfpn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zumdvkbm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3enacxjbk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3txrafrql.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zwhbcllg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wwzywfxj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mnskwsxa.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3iggjawgg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ddmkblmf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lepknqrt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbzsmzby.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bmhcinty.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iepggbjj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dtcfmjmb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wpxcaywo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gwqnsmmu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yfgvjfcu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ptecxosn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ggquxisi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uoechoop.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qjrmvbsk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ktunzcov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cdrdoklr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofipxliw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vihaovzo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nhxdspra.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qlbwyydx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3saxloove.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwogsqjp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zokkqrrq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kjbljigr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3elwroibl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3illgknyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogmfcedq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3laelznbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqgemtso.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydhvwnri.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jektofha.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpaymgii.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fugavmks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3atayvwnx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sptvwxkc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pggbwdja.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buzbpsbp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aodoiqll.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xuyiwbhk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ddnrxrei.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bakniknk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlmzsvfa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfdnxagz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kfchcywr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3abvbkplr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tndoxjoa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mhsoefeg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3pjmdlhvy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dlrgizba.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3anvvnvfu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3awrwyobs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vhxziymp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xbfzpdsi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nlscfefo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hninvyqv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mptwdsfk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3iwbezrqz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pikfvyel.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3msjiakgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jlebngbh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hdjcipxc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3chdrjksm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mhvyhiho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3luesnxcx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ngulrnlg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tkvumgro.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jzulflbs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncsjobst.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qchsytdh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ooprzltm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bfgarluk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xdzncsaj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcianuiu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpzzoahv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftcmaehh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eutbmlqd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uswaqjsk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxevijfw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvpjbtpg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cmdkppkb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3befprrgu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfbytvzf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lutixqiw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sidaiowv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lxcnovqn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wgpfnhsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cvmthqnw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fnhxcada.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wptouzmj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3alvcvqhy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3omytjevn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xlptrvxu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3khrhqvlv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3shkiboxv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qtckwgeq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lkyomqij.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qbdwfehd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wetsctqb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fsjhdsws.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dqaxywkt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zqmbqmfa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3takntgny.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqncxrpr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjsggdqj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wcpckwbt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wilebuxa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eedgvwty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iswenwmd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yydquybp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vdywpvcu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uwltxoqd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdhcnbud.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jmxbvbma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cionngnd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lixnzqbj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hdlvzksl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldgrezie.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chueawrc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxcnpwkt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qilpjoaf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hswfemoz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gqqhtezc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3utifjgfg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lczaeisa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dmgrroau.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fybqitdm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hftzwsoh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3skvpqbyu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ibqvasel.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjybksa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uuecjefu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oaywekgo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ajqqsbrc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3evvznkbz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wyruqbnk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uouyxpjp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qunvbseo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afmckgth.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nzafftjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3retnzaeg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jpuvjvsl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cpzdniij.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ahecbhrs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fqtmpzbz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bknlcwxo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yplxvfkx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yoncxpvj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3usinawwh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vjlyuxzz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xlmbdoai.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3olmvuyvb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dfmkrcjk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmlrpqd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upcjovwm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpaocslg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fbbupzev.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbpnkpsb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aynvtfwk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pnfhrsdb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3guwkezfg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ghvgrtkb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xuopczoj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vgiomosj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pxmoyunb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kyfeazif.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zkaxppsg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nuafdwxi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lduhtxor.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3flwzetyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oxdtdwep.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fombnrjt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3voxviuml.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrrjrqrh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3woaempoh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3toygthel.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qasmyqmi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mplnnriv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kprqhgps.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jwdpoipe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fminebzv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkjlngxl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wmkujdes.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fsabcgot.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xylwjpdf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjaxabgl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qgmixiph.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vapimwrl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtnrdnis.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqdbcabc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3soxdkhns.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rqmfbsom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oucmkgyd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ibhugnvx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ehepzpkt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xbmjlmpj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yltovzro.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3afkgeubw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jrizjlra.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kwfbdlgp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wklzmiyb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qkfidhzg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nzyslaog.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ywoejxuv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sbseqrlz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3djrdazaz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mszjuvyu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3drgnppxl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cnnwnvfl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zxnazxfi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3aopncpre.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nefplyxs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mrpkbzkl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dxdicjbi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nazqizpy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kxkiasmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pinweoxa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fznhcmiu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nohgpyit.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uvfutmnk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pzrfdacz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbkdlzje.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ngkgjeai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bfjmjkxi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pkvoqdao.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lrkfhjia.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zpbyazyx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ioybbkyb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wqmilrnf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lqfxokhc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3aaclosxa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gaebdqem.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gjanfrex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3smutuptx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmsndzo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkcjpzv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gecqeuct.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bwajyavk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mjphicye.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xflggdbk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjgczjxr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wiqjdruj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gdwqwryy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wydootqo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjtqhjpd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qouhekvv.html


<!-- 参考信息 -->