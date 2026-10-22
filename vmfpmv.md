代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2gxgylyfr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ioauwuku.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wcfbhgux.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gwrrytxy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhthomkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tofkaoaz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2sanmbipi.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgkulrrk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tdopdyql.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qqauewqt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dxdjdrbg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tntqyntc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwasnfzq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gnesumvq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vzhayvhc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pvuzwdob.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xkcjriar.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdhhwblb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqkkuka.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2anmritee.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2apdzaife.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gtpismmp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bauhjjeu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kvkdcotn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tglimrnd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zjxbharz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ygoiuqcq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hehpzlvz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rnwvpxej.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2culbibcr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wnflppun.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ygxahlqd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eswitxrb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bqokunhx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yrqtqydb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yaadzyci.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lwigcryi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cfevajbb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jpjtecwl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zvhkenll.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cvovnjib.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2idjcokuy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pndlzbuz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hasctywe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jlhjmgzg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hkfeyafe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2prkodbyw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yakydabu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rjywnsfn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vhbomdsd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pdjndwea.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wwkkykcz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fwiazfyi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xmbktxwh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wqzqtzbu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vhbvqevg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nxbagfjx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ucpyihbn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mkvdeofx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jnhwomkx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wansvuka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2eionwtbp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2octbxssj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejgkilmo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vhdqlnoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zgpeauyd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dbrdvaji.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fsfjeohq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pznnbhub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbhhhwtu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vmnjfqzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmlqqkzg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2eklpgtpg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aepdkyxd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnzluhvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mqakdjzx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jeukhbif.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxpjnoht.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oltfakvd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpobshdq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umvprfvj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdxjxaxw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bbkbpexc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tftcmxxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szhvgkfe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jppxwuxc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ealocmgq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmirrfa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tkrxecna.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hceszuwc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rzmzgdyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljogjiok.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vmkgfsvt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gggstpyp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xmlatstj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kiddkgkt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wkhabexl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zrmejequ.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2amqzmgyf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzujvvtd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjkziulf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2euawwxll.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2guvzduud.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2elvoawxm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uninixbn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nycdcutz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2krgrwdox.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2taxqbbyp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fycflkhn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bagxpykk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aojdwans.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yyfyqhqm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejilowyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vthulgmf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qnlerxqf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovpllope.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhdvlpfp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ndirgpff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbzicbke.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nptizzlr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnwseber.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdarpau.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgdcrmhs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eisjnhiv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lprfefim.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2icleqhlz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sxahcmos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nndqdmht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kwfdfjst.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nikluyit.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yoklbicl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zjbddxxl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rldxuvmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2utflivhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gkivaiar.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2byhwpjxt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2beilswfs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ezkijfdf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fczdoyvx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwupkntj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zltubcsz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qvejtjld.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vzuwyjth.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2henwyifl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2awkmerkm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzxezzhr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flsphupy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tepehxcr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2irnhrahd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hrbtqwdg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dsshbier.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sksdljej.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ivjexjbh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qngqxxfl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmkytmmm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uonwkbeg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcsaunhi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysfsbbaf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ghxlfboa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezzpkbeh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mitxrkhl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxplcswa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2akmeanzk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tajmzdzn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fxibjyvs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvbaekmd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2usgwhywg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fggmbzbt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ubxapqbp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orzrdtgs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rniqrbfu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hppnqvgk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pwislocl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gvrtifqi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uasxnvkz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ujvkqrcn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vxestkqk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2odnqssrh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jxkxtxfn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qhhtxhyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjexalie.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nwabhrhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhopuahl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dfwmoxfw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jdlwnpjg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tqmzxrzg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aixugijj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tfscwfdt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaabsihf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2seshjbql.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2drmlxpig.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubawzodb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xvxtoklm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lqnicomp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zlwzbawc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sgdhbdaf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiuvifsz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqannipe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zcpqihho.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2muaaoonu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnuxucxl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oetmkdky.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mgfdyqvk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vhcqphoo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2phjnygsd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jhjkrptb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dcmvjojl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ixhkaaod.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ramspptm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wtgjvdhl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qmitstkv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lvdnbffo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjvchhwq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kawjtjas.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wwyfmgke.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gtqvpgqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgpkhex.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpndlogy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2scggavsz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qfjdrdmw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mhmlsbzr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqlrgpch.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mydlywnt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oinrcwyp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2buxqwwap.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ztxpiayr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yhokzrnv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cprwcgmc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zhphnvha.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zchrrnvo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znuqxinc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kkowzguv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2azidlxdk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nnrepfyb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wrhomqps.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xcegwdbg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qxfllbff.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2awnnrfke.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yquktahx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bbrofjtg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gygjtwde.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ukhbnzst.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lmofrene.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iuwfbaaa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2awgopvzk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2imsatduh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2swlzzhpz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cpazpans.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bcklzfgc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2evvbmeda.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mwzrroxs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zlhgoqbe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nhyygkpq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixcysaws.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kmwnkmak.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bcevfwcu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dptjklfq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpebxecu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ewbfsxzv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2toqcxdnd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rsljvmtb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hlklifyd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cwfqxxqe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yvixfmtm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2htijsllp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sfozcafa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mrbmxjsz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nbjaqinr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ifmgzhff.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hrbqjdrk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jsylxuxh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2khkimoxj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xvazwhtd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xskqrqpb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jmrlqxnc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxshtpy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbwkmnhm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zcoethax.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2obieuuhd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hxgmdqty.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2idiunmsk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdohtmzl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2embwdwgc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dwuwlvvj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2huvoktok.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ecacdixp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2luldtgzo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbvmrxew.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zqargsuo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wjqbeymi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oriqqwsp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gloxgmxf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ocbsoueu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lpcaukut.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jryoiwxs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gpigglpf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dskeuqqh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rovdscbp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xnkfyxrz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lpblojjj.html


<!-- 参考信息 -->