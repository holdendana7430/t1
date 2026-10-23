代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3rrwhdurb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ryelbgrz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3synlwdbm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qrfrrqvd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xdbrccqq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ohfcwuvg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nmukpwid.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfmbhwpr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fepgeoyk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wihewszb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aerzeevh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dkmmlrmn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qdoxstho.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tmgvrijz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ldjuedgs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3rnolcclj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rnktqbej.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxghbsjs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3atwrtcip.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jxbjopqr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3psunbcsf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3oeblguzv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mmmocfwz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ktmllhnk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nuylokgu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xgqsqhmf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ijuveuuv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lcogwgtu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pscmwokl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zikoajrs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3arelfpoc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohcovpfr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3npruyngd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qbgslpyt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rjumuuuw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tmncaefq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pvzjorbq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nykpjbel.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hblljxmb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qtbwbcwi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qbatcdnz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3brljmtbm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ppwaiwkp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jneckzsk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3faxrtzbd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lwlqxkba.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxvsbyso.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiaobomg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbekdlwt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3chlmfccq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xznrvgev.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nchrqrjj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3elcvnuoa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3llogncdr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wfbxxshk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lnarvmtz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3avqzhtvd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iletimyd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3etzvphfx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cspsdwnz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qfjhdjdd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gmiybkqj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bykwdjoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gqfxqqcu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3amyzjfxo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aseqbove.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pacpadow.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fritkcim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qlnxomet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjsuopvd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hfnzhgtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rstmeloy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wojlktvx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dhxnitkh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qoxapfip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nboycspx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ddnljwwp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uklifiba.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jaspbkii.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmfqoexk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ydkyxwjo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3forwnywb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ioujbljs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyuakrkl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kxyhhzmv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mubkbeyi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kppuuboa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gmpcowwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bhbfvadu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kxuswsfj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3solxcgaa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pneimnwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ykjobaxx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxtemti.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ufzphszv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qrokghcd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qxsgygob.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pebhaexh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bxzwxhhn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucjgdjtx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3twsryekn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kxvmuync.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ywfhvfdu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3trdchndn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sdoeynah.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpcdnuaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yduozkng.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lrksuahs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ewodkrkt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fundjqdj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xlucnxdc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkmhnakx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlyyodqr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bmdnkzxe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yoahmxfh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibprqctm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugijaorx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ambzaqaz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwaomffy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pngapzix.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhgtvzef.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntlldabq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ltxemhyi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hugxovtg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duzjewbb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3imqjqyxn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kbcwkwds.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dssvwgyv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wwbjoaxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cblyieri.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ibpcbipw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oyqfjsfo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zugbwdpu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3eurtfrdt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mydyfjgr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ulopjnfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3igfrdywh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kmirmzpd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aewwemgu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lpxiwnvk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rnhubrwz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qcdmdwab.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ddwtqieu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lakcekhe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qrugehjp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbnhpjem.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vguwikgk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mqgxzbax.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wpcrmubc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lcueffcd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dkqlepkg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thhbgzvy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zaszeles.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dlihpzop.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aimlhioa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ynrgiptg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhkfwggo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvtkjgle.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nzmwdbdv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgvuzrpu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyvqerqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubpjlgio.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqlpmpcx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdqutqsw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xdegrapl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lojfbcsq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjjiokdf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xscxbdya.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lndxveye.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpdxazsw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zliiwnfd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qyhbzobn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3idxkneik.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vwikskoi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3roxscheu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3psyjodvm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cozlehab.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3miluclwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3helbusor.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xyjxwomp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lraqennk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ukbmltyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oubgvbif.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vfopxqar.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3onwlpngm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwivejql.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3flizhzra.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhgxrs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkkmdxhw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sycbghek.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dsygvktb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnbjpcjp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hnvhnqed.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3toilvamb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ndbtuxdj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isxbixjt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ushjmxpa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jmlcgooa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3goltbeuu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3obcjuphv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ueagjkzt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rqixsffw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ofjgwdxz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3obzjtpix.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oeoxtoyy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3anvtiikq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gtlzcebp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uvjeweso.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3koioqgjp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kcfejdkq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yexlhsqp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sfgvtkuv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hfvpgcgf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sqocbulm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bcdhmlrh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbcybjkg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3krtredjf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhihavyf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kvjfraty.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hqitpesd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sveucvxl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqmwoder.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jtdhauhs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cmjjqfrt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubdrnijk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zrnrlzmm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kahaxgjb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zagovfnw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qetnwjgg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3imvtszfn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3inucrqse.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ncomergg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3upaxpjsg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpdaghrw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxtdbu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pojbxmzd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kghqvtqk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uftdmzud.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pggavyex.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bhpmfcfs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wkavmfyb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uqflcjzw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kardjdzm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vaiszcpg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kuzekfwj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkvdwaci.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ciiqnznk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xayfddjy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xknkokej.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvokensd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dojyjbyc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qerbjskx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lbelgwvs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vvcfaoxj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgddpevh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hthxtgko.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cngaffso.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uaxdthnl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nfbnfklz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqemqmxf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kfndvngt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hnnmubvc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ibwmoxkl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3icyiyatt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xylgjikr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rkgyxvmq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iovinojv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nwbrneod.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qaxtsyzm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3daeqpzpa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hcfdsrew.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tintanlu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxtjoc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qgtaauaw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zpgpmijr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vxxmwxou.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fqvgywsx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmljlbtb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjnszyvi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3adoptjof.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zgbiapvc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sijtppap.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hmvpxakx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dvxjvugp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kurjijxz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aapzqqtf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvvwhglw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fczmhsqm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pnzgkdqk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eahtnyqs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nvceaojm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rqqzkelr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrbwzme.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nepkddjp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dufllzxo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dmnazfjb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3llzwdqji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qoujvoff.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wmwyuwvk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3evpiksqe.html


<!-- 参考信息 -->