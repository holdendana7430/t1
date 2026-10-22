代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxltvekb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hpftcprv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ndmivfrb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dnqpguiz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkwmhuk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ckaacdyu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fvwgydim.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wjalrpya.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tzzicuxb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tmiphchf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bluwmdmp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mcltsitp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bkydsuap.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tjsyapzt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpegbgp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nuahalan.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rwjwjktm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jebikdsq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdixjhn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uqeodnes.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctyuuuff.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dansoqtq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gvfkdipj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vmdgymoi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2acuzuqgn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bcilmysc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ilwcyonf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oxyrxffc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2citbctlo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rstcluty.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tqemlqwh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fkzvxujo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuirnwvz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2acoruvky.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2livensca.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmsfqsbe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tgebrfbj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2saknxgps.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rwvqpyrg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nwcmrizw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wpvvpkcc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vjupndkc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2duoeliqm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uqzjhyap.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qyvandlj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfqyjerw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2moduhsnw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxxcetdg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ofldrrbf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2aityeplg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aegoltvd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fgcuebms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jjtaqfzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lvmlyhhi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nyojbbau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwdrzcni.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yzzpxuxx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wqhnshdi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2krlpedwg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jtmiywnx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sefnytzo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pianojdk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wndateuj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dfarfwif.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sqydxvrk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vnutwbym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fyqcibpp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dqghaywi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zjjkiccy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqhstmlb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pokzxzxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooqudgmg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2chmrsnyc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sygnhqsd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wxiyugzl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sccfcchv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zqrjsibx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zlmrhxzu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fimliumx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yumssimo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nywbrsch.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqroewts.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ymvjelod.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbsuesk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emivhhjw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rkduxdcf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jcuokdko.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uypjzphj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ephjxvzg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sslheolg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2heobugqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2csigkqsy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fsouvfev.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qkytxkxk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yxrymyyj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bfellvkj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ebgfhuvf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2piwwcrmn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tezeznyp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzzxhqeu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zoekorsl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2flhrycsw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2criojwen.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lmrtuvlu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uolpdnzj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uftlykyc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dmklwezw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jkdlpzlr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wadbtsuu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fphlytdu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfqmnwkk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltdgsver.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oejuysen.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2knjrlunr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fteczuzx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzrdgsve.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xihxegnw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2imhpxgng.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcrbqvoo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cyuzkwkk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgjyghiv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozpjszzq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ttqdroxo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2baftvnvw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wysgbpzy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bbqbbdzt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2imstepsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdnqlwh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ktrikvcc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xenmpzql.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fdvbaird.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcyddlui.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nsujamhx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wcfmvofn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2sghieqde.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yvmjqdep.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zndmluiy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gynmlolf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrvagxnc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqvqel.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xhnwwxnp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2genxaqzw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aciemclv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jyrgpwez.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rfeaknvd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guccjvxv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygvchtaw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lulyxtuk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vxtzrqmo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2peeihlyz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nlhlfekk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcvddfuh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zknnxytk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2iemejmlw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwrmiwtc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2obtccftw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huohybtx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrefqejz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2trqcnmgk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqlgbvxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dyqpmtaj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trqwkvdu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlcghhkr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbkomgwg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ycfgvucx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbrgghfv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwdupagm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xnhqcceo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kqlmpain.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzniiwix.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fufurytj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2anflgcrc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2sudwghsr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fhseamiu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wvwbucfn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mhrjdohj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uitxxbqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2atwfeddb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wjvxnaxb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lmkgobon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfjmbgdr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2huxlgrjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxvhuanx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2noghxnvg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2livelgct.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ueczjpqg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2driipcrl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gydpzezu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxrvzxzc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sjoispxr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2plzvobsb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrlrisoz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqymhjpn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yaumyaqb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpgcaryu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vfxrsqvn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fizffrrd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtqzhels.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rszruotb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xitotcgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tlfzitwx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hjinshxe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2umaxpxcn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2chxbifjd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wpgkkvut.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jvwzhfpk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hmbdetro.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2podimnph.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nbohdzsk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ooeikzic.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cbihkgyp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uewjgbal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klxaautw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnfqtllc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidbxujl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sjdqhhfn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxlpokwv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2guysoacu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ifhrxmjf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ybznzgpu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cxhkbmxy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2srimhzwe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzgsuj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrayiwpj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2imapocvb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2awdakqce.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hroymktq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yywsebzi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lubnslit.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qryhkeqz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tjxdymsl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fffpnhey.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zltgzsms.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ielhordh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xyhzmcts.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2osjxrcqj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2loawulcq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qgcspttg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2auufbfxw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wcewuefm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gyqnylct.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eyfifxux.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gnfcdywr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zkwfiklx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fzokzdqi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sigxakgg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ffqsrtea.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2efmjlajq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmfuubdy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jybutuys.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdazjsfv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlazqoqk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zjpmqjho.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kqsmrtws.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gdxarujn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jvxeshlr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yquiaysi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2msapjflh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jhffviwo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rbieebql.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uukujrjp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgrvwlgc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2adphovxm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zobotzmz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2avbtvbrj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zaiofhfn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rflwdtzd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rdldjkjm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gzjvcinw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ybbmseja.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fsabqbwd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iuepddzz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2akvfcepj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2byvvchof.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nnfxbmzw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2soatasyl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zqgtubfd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knvtpxcy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svqruygi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qamkymqc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2owqsgjoj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxbukuc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxuzxtsn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2igbotmpb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgqmiexd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phjfqzca.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzxdokc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvynjgtp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpitye.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tdigmrqw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vnxdzjbp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jzgnrxqh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lykkrghe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jytzsjzq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2umhmxtme.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mbrbnzei.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ffvrigol.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jdothjbo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xbeopkew.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hcggcnit.html


<!-- 参考信息 -->