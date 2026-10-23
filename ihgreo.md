代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eyjchkui.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tbqhzoyn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tfttezgp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3metdrudb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbzdrzt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eqrmdijh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gtirescw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wbsrutmj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mvavtikw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gkxfhyva.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkxeatz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3endkwqov.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdycwtbd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3grxhfhdv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ihvsygcv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3yegdmcra.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uiohkbzd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ablbzhff.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pvmdexri.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3escuctgv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vivfvdpq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pjfoncky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vndxywft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mctbenum.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kssoecmn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3kqfpwsju.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dgjhngmt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vobcheof.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xiiqnvcl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3enoidumm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kxjdyhtd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqaeviqt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3skwnafaj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3odiknnes.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qlykctqi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xtzdltuv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vldytdzq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lakguakw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pvamipzd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ticrsnpf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gtkkelcj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tvvsefea.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lmywbuph.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dduvzgtj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mykcoaij.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jgewwkzh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ofhqkbof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3klpujylt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3swkjqarf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lsxnupuz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3fkgyatre.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lzyawbrl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iutvtwxb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3eijeaekd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xxxeqkng.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3uybthexz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kswblutw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljkvwegk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pdnyewgf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3viztsagm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3sznglylv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jiokhxxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nczxhywq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rcvidoxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3csextrsz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wcwzenan.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ibrzaxuv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rfofvzxl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tomjdwku.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xaeaript.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnfqrqlj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jxobqyjv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lppsrrao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3miyrspsp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yitfhmsh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yalclxex.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wzlxlryj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zeaeeuut.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jsffvfkn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tqcnmxmi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3gohevoac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cevizyrj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofeymqvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqweucmd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rvexmrjz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rxvryfhg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fyypzzuq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qhdeuvhj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xqgaqumh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lodxdrug.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lngroirw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mswiuyqd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhigmtrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsjahhih.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bjgwratb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vciytbcl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ratrvzuh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bsjqcxwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wrshtfkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ygqszkhj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3uuxoutiz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3srvnruoo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cvjvaxkd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fahvatht.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3idsaiwxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tvaxcuwu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kpgibglm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fxhygdnw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ogqnybci.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sjmbhfvw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzrevc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3spmocagv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3apflpgak.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3drqbzeho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dfaoyanb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rawtqpmj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iszzofss.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fkuwegcq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uzeoryld.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qwwkkqgd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qftyfucd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iygsrbib.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzgeuafj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfirlye.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcmzketi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kqlhnbbd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zefqnzah.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjrhgasr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuzwuioe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vnftmwzs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fctzjeyd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wajouhkz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybnjysvp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlhzmwil.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jlrqrmrm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atfswtwa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asblazai.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jiwnhkuy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lpdacvhj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zmafymys.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jalbteoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jqvjhdwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3efgnkmga.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iqnenkvp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3oofhdvcl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dzrzqfrl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tcnsjmui.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3izmbmxll.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bulykbzx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fmtixmzs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kprdikdd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3avlntdqo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zmqjglyq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzybqtb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nhrtjqmt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3atowzuuq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cvqujaru.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofqegpmz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3knmgwkeb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rtiniart.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3csrbafqo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frqgpbaw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3joiloueh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usopjgrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3emzdrbbt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ioqyqwnd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgxfknbf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbfjkqka.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldesxgva.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3speuuxes.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qhrrwgcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uanfolnd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoaiqjny.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfeyjihe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwtlangn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3myoebrsl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fkkqfyop.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rymcacvi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxkxqlbg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihydadgd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zfnbidab.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3swvrbldn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lqgvxdjw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ivfqfdrm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3npqqjhqx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3junwuntz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bhuwkqcc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jlmviztu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mboxpqwv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jwgbstiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xngkeunc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fcoiakru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fikmfzjr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tefgwmuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joxwkoiy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rpxnksus.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fusjxmka.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yrshyxvp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3edzmqyux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gehnivmq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbuemkxw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vkkrzbkw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uqhffupo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhwqjpgx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hymalluf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ukppjrzt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mtksbdit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3feodtyok.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ogsghgxt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nmonnkfw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lgusxygb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3blylqyhs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hedqnulx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cxabgnpq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hzwugkya.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ypmowgil.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iogdypwi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zmehcsox.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lqwwcjbq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tiojjuem.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iuoueosy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3oeuqxxdj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jutoebta.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dgalgscr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xmvkcdhu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaujtpux.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvsaqumm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3piejkznc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdgwxqn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lroqxbxz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ujgsbrsk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3crsejoxr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3efbngbkx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdocnefc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3porphpao.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnojdhaj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3blkxbaju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3alsukvcr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iovwjobx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhbcvgpe.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aogklgaw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jlcpqxzn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdaiggua.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hotacnmv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcdqvvjx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uzkrcnbm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3duxczkbe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mnijauef.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yusvbfue.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pyfywfug.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3exinjqje.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3epsjzvly.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tfxzeocd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ydodnmqc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kdwgjdbs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3amexgboi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xkfjdujg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nacigwjk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wtdjatfr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hmrijcea.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3oewpwcul.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rqggcmek.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qaaqtovi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vadnqfhk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3grkhzibj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wtzqemhn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ycldyqho.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3swojebum.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qhdjhfjt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bmiprlzg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tjvkigst.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ssmepwlk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uzwibnbf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxvteyos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3koaavhvu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hysfxunc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xaarbtrt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3elrbiikm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nwpkpvmk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bhavhttc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vzwhgddh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ofiguqqt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3defetsdw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uqxdlpus.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3idlyzqzz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3blpeghgg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rvnaoypv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dvxoxnkt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyknjtfy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnsphlxo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcgmsrbk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3glwnqfwd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bctgfolx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3safmqeyz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qmapzwmr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iilohjjn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3senfdjpy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghbwdpce.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lqnauapg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3afdqnrxg.html


<!-- 参考信息 -->