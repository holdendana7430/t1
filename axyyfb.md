代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wpwuonxl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fyroygrr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axzsvryj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pjdgjujz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnebvago.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2psicktey.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2igdtnuxg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adkqjskc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uivhbujo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqnvknk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nqmyloui.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xzwrrmwz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lzpmfwrn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uglpiyac.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qodbckfu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fczhagip.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nuuzktmw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2iqktciit.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gsqljtog.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uzesiwgl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bqnslkag.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kevliatw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hpuubbcm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mogiikwc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcktqwns.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2seslseuh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2asogxtxc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gctgmhpf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yycnnehr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xlexkghl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ajphbkqg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vfskdifn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pixmujuk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wojdoqen.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2abatuwxl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2idhogldq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqeircwc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vggtfjcf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lnswqmnq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aicxenuv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yduyvcdc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xkoxmech.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqzplpyr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2boxkcsbu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jubvjrnx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fkkrnmtv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mirnviow.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hfhonknw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2skvzebin.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2achicfhj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjuzqak.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lhyckzgb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqsigely.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wleppejl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxnxnylr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gjkdrccf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xrhavgol.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ixhmgowa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aerzkobo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qpldfgjc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ouzgpkrq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2suwiqhra.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qypdpsxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aqswqciq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mxbmcenf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ypccwesm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fteylyfs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rgrcscrm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fxkgttvs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wggpzcox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dtrqzkkm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tczxbkww.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fltluxno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtkkriqe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hzroubmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woihhnjc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlfkuifl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmbxnhx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2utnnrldv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rbpeoixt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2raxkyose.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkljaziw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2odohwkby.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwfwyyjk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fxqweucj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xxipwbpb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ygvvqszo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kawusmzl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wrptertf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lctoymhz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tfsrvbnm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2actrjzur.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fmozacec.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fuukjnlq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zowktfbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2maziackk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tyflgajo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jjtiybaz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hmkmxsmv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ijfuclfh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwvrvfd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2guujxwey.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fmstjghw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hmjontvi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jwpxtlqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ovmlvktc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2afzltdmk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2klwhoizm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cwunbiso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vcvizffn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zldvsoux.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jeqsfkci.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jcttdutn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rmnrmrah.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhuayhhg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irwqqdlj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xasahiig.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2orguowxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmejozo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhqzvmrq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljuigwwl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcmoiadf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eatksumu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rolnxrke.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oaowpwvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oktfiosr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pegynchq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2appvtjzv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqpihoef.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozopimgf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jrvedgwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dpsvyzgv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xqwrhfve.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dfjibjno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zkyevtyj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yyubeqom.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uudcipbi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hhdugfmc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2whauvnsc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2shhghyml.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkscfah.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kdbryife.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uashxwoy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hdsgxgeh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ndfpyczh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zndjwbuw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lmotjllj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wilfnknt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2smmgpovx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2duvlnrli.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oafxqueu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ffamtxoq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2krjrxuoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tcrpfjif.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qfctvvid.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqvgldxu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fsbukxsq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rlbqhbhk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbnpeqzl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhflxtxe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzxrddda.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpjsrtvm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jtaazcvo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgqfsidr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbpkldpg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnpodotq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tlafsbau.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iylvtqdl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmthzmhz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnbxkpeq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvukwfxu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zexabjwz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cxilcccd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozxaxnmw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tshlhuut.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mhbwqiuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vtzxlqym.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ngkljqxp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ioojbrgu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yeainiit.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lvvgrnyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hcxrpetu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ptksqrze.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eaxcsyya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yirgeqpa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2roevfkvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fipzyigh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2eqlebwch.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hdjpjrei.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikuwdgxz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vbnbyfjk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qoljtnyi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnkbwgyg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wfavpwrr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvcjlijz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiitrics.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkxogvcd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jkmcnzrj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2chhwmbwk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2csqsqxuk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cfqfmaxo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ttkycglx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2scfqxvzw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jltzsjox.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oyqkszlm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2sfzhttqy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lxsgwiko.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kgfttgpt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sikfhcyv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjhzacvl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eqiihadl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dxpwvdbo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uijwarvt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hdjdhrdm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gyyeyfpf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cyodoofe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiukdzow.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnjadfnv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttvcvehh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nrvyrxpz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ejxdgsfb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjbppial.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvkozl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hkswmocm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ezzjeaxn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2okedkfha.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmaowlpj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocwigvjl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcxetpvh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qeqiezao.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wawwpapi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jytwsrrs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hepoiydu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jtcdoxmz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djsklxbt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wmtodvkb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtotzmsg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bdrmfnat.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yvivpvmn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ugqgnotc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wpavipqo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2siptdmmv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qlphhiho.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jcoohlch.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2redjucih.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjxsaqql.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vjwmudoy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2drkrqbmb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dujvtvma.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dnivrvce.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sxthqlpw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2krwgsguk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2alszcrpa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2izdrpcfw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2klnuiocc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lapzkvud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tthuoces.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2nfxtxghe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2phfgmuli.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bgyxlvyw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kptguojw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lgzmwafe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2izkwtfvj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hhqvnfel.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nrysnise.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qovxitet.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hfrsowzh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mhaxivnb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yhormloh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ypycjynh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgcyjidr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qsdfrtea.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eopkupjr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2prcysofa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kbsovgeh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tptramqd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ccptnznl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2becounbr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zxxlaysk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2piftdtcp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sdrqrcgm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zjqwxfoz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dvjghhns.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kchvfpgs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ejlpbcdy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kphftxtv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jbpxavwt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2klnnrxmg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpjpudyn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivrynupy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qklhbexs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rkmrevvw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zufgoykm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdkltclc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oywrxabe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2appqtxtv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lzmazwop.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2icolfrmy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jkanltqf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cgyyvatp.html


<!-- 参考信息 -->