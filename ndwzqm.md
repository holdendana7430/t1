代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3diehjtul.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qpryogkk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lexhvwyj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3poqqekvk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3feejgdft.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3buotirih.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3koefetgl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rjkfvmsa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gidkrfjy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3aceuiixm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ztcxoroy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3siqrxpmt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gtsojjoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nopcnkyz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3eftjscia.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3kfpndpdq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lvvxqsok.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qoodewpa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdrbmmes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgpisqi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3jtzgrqyr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pgazylbf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3izfjelnh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vbznzmnx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lpqejkjp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3cpwittdm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3mtwmyval.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hcvnrzry.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qmidkczo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wpvhcslm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yziuvreq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3svidgwfw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kysasfdu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fuaaavow.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dixvfxsk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qrdhwviq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fmklakus.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pyyuxkam.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jkaijbdg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hytxfvbe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ksecapnr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bsnyktob.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nbegsjax.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bwyiicsn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3vrbzmbxz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnbkrcvq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jacjskup.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tufsxgkb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ihzyomhd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ijxdzjuk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udlpshlp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wgzlizxt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lemoerif.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3utmggbtb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ixtsfyzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqwfjwxp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hrftfexk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3enbqhnzf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eizvlthc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hstuigrl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3avgwwmzv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cbwrnukw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jhnnwlot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pyudlpkv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3njcihzav.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ipiajale.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xghfmxpr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3womoewjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jsxonzau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhqfewoi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fllpogtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvlcxchd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3okvehrcg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cjwryapc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfwqafma.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jyirsjsq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qydbfswz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ctqonrvw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ypnlwsvh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rastkznv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dygpigfn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rahrlfbf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lsmjwqso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkyuzvmy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvodmnxl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkiutwko.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3euqoqaiu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ojhmdtog.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vzzyhxgq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3poxwdqau.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3busmyfxk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ajsoebsp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jubdkkke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3efdvxpad.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ixncrtnc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sfwgmgue.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3okxtjflz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3myydjmag.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3traxptrl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oofwybxd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vwnyhfeg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3funybvlx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pezqqify.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yvbmoasw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqbiazs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xgibngsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdcilgju.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3oooblpru.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qfpvlnco.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iltysbaz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fgvibmsk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgwayncx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odaedjja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cnlewsec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dqfxtvin.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypiwhlzd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tziqbuzb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxbvckqb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wskfojxy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apsiggtt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cobqivqe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjckuowv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iriqcogu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxvseews.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scagcirp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3siqlwrii.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tpawqztw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpywgnr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqguwbqq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rtblnquw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bluyvhtt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3scnotfvs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wocddzjc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xppwpdga.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lsjkgpcy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qwygxpqp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgmqvxs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3yujggzgl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkvvqui.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aeupddwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ydkdltjz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3srzacbrj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lfagumha.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ibssdodh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ebsnwtam.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgxkefsf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vibfxkwd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iyoxypvp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cfonfgxo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ithvwgfd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3btyqnvdh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsjjiphx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3avddqaph.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3folnzxll.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsatbjdv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nadbxrsf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gndmhnfx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flarsrje.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3amydoyli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3barlkiki.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eleuvcev.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxxnaohk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyfvvzwb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwpgtimo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hfgkdpdb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnwrfdss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3waunevkb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zlcujkke.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3unhhmgyd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxephhte.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kqrlkcqb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jjunnhab.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhqbubx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3emeyseeg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pfpdmbce.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nudtonff.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3erzomouz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cbgrqbls.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hiamwfuz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zhmvmmlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvnxxcps.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3krcqdicv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsldpjow.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3strysvdk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rafabsgu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ibwbpbeo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oejdrfzc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnsyctm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ksjptjks.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ranfbgha.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjhrntrx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wmeivvfi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3etpzexsh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yzkwftbo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jlcaizbs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zequiodw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehmwivmd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogqsjnqt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mxepmfoh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3atwjltjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szbekdsz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bfhftrza.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kdelsohi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hvtnqbmc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hnhbofcp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3napkcpit.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qcucztat.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3denktwvs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dqbjbxla.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wbqiftwl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eyxqqjpp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3skwikmzu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fvxjvllb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ztqrzfip.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbudita.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zleqnntm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fkggnqhc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qvielulv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xjfylwzq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xnyuqfbj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3skaeqhpn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jejcqzlh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lumlizwz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzdsjuww.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gwaxzlxc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ftcejvjy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wijltpbq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3prwjyqml.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sbqpkjef.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gwikzcxi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bavaawak.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjafrttc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ygxygldy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwekkeoz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vrkooqqk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3spmrgmuf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3swziinqj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ksrupvgu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ziliorel.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3avzskzqk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3omsoaohb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bbcntytk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gwhnbrlj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3afwrrkrx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hpyxvgbd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwzvwthz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zoslvhnt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lvffqkfl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpiawtzj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kntiyypz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rbdaivsz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iswlmfqj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ajmagdxs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sogyotcv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xesuvcpd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qxlsbtug.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ceojmumy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ilwaxmdv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dozkunwv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilszymku.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jmcrtgqj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3udzbhecd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fepgfmqo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntztroxb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uvcapmyv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nbdqgleo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xlpgbwuk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yimwppvt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bxbqcdgj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ycsdqqis.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lvphpirx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nrxzdtcn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3shcvuhxh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bfrzvkmf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3weukwztb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nitvgwvx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofuyswap.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eknghvpq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zozyzzjl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ancohqva.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pvpkucko.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3takualpp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urvhwutt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ykziuqpc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdseuij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dbqsdrvg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmjbxhmh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kyrfbomu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ntaxqjyh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uaavfrpv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vwmsxcit.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gyfovlza.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3madqcklh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wskumdxd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bdxydkhv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jawmnspe.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3guvcnsaw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hoyebdmu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lgtudfcf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uunsehft.html


<!-- 参考信息 -->