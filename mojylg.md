代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2llfkfiln.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ylyxdbkc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gklxttqj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2emcdtfnt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bahpqfzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhjhehc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cbrtawmh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ovlqhdsn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wexpotfz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wvgpnyap.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nwvydahf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mjccgdxn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2shwyleqn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dsbzihyo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dsjyphaj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xdvtxret.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rhpuxrau.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ggdarnps.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zvpzjkid.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xrokcnuj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zzeqbvya.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yvuhwvep.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dwipmuee.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iavxxpst.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2raqawdzu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqbatnsl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iwkyrjkq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rnpbiynw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rdnsoflx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2stsylssi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bvdzsfki.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwnwukwg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdhvohz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vzuuxtgu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2sbhczrrb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qrgxrpox.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kmqqpijp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bzyxcrob.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2khniddir.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yqydtiyh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ewkkjdlb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nczjfbgj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gmbbiawm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2awncnguq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtnqxuux.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zlnwuuwa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2etvxskop.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rfhzwcqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sxluwcmt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbtxcgsk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iihmfhij.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nhgzvyjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jucenoym.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2uxvlegqg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nxouxywz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hauyzqpr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yswdhjqg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2atpvsgpj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ddsjhbfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvcngszd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xtfyciip.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tckoolcu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2quuibtqq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wbvrydjk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yhqqcpaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtghferi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ugklzgua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzgxidkz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cmyvuohy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rznluqzr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lyiuuwng.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxdkss.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2chnavdbs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwkfsu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dvasuddz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urxavvpn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oytyeqfg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jexuctxk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mplbcxyz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vnnnfwgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgrukarp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sesqdubk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2icsgywzs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vgwifrao.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xmptgtyz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wwqamnqr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rtztwkgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbzluyi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jrzezksp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xdlpsmxq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lghtsvey.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ebrdzvff.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2laopjmsq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mjmgdrzd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cgmfcfqq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fnleront.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lrekwjbn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2imkizyfj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ympqekru.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oqgobhnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkqtjql.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yywyedmx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tdshpmlq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2azvzgghg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gzofdqky.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vyuuleef.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdpcydyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icrnlesw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gsxobmnf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lrloirgg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vyqedrmb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmaogtaw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qejhjebp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2sydkinvw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdttyni.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfgdsxzr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkcfogwa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adscedos.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxnzsqtv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnsnjzqy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niivuvsa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqczdotr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2cptzvufb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aaiwezls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2skhemjen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wvnflqdd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mnmstwex.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2itrygoji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qmxbrhuo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhwgefx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2flupwdlu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iatwdgxo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ftfbueci.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2owhxpdlp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oypsfmhm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2amyzjgbb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wtwlorpv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2inlbkbww.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwifgxet.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fvgaywdw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bsebwnoe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akozuwsx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhxkfhee.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2svlomvhf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dgqbumrz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqsyitdr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lpjikkok.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtnggale.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nlrmrcue.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2flfooydd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkakgswa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dejfjpps.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncvufrmr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlxnmvwl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jrvywnzk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oduflrci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwpcbzou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbkiflj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mvslxyzl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bizysfvk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xzaqqozs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epkfjfuf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2panmwtbl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhwuysk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jblrfshq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozfhxjyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbouzfl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ygdqfmma.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wrprfrkt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zkcmhqal.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cpluhqel.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vbmeluxf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vdqqedhg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jmcqtcbl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qxxpqbwe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ruroejie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psxuzayx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uzgsvvsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiwftyko.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2liflyxaj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2htaqupty.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhjxjo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhexsvbn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tmmqdnky.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izffmsls.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vyngqqaf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zlpjmufn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hagbcuyr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxehaezl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zuhowday.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dhlevuzg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kchmseag.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykytndit.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqgwaafs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dgaesova.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpisqtvu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dpvhkvow.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uzfdwlqf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aambisfi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mylzqzdd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2voaxmael.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ervbozjm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pntafuib.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uxgsynhq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2chgufbyz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nudjkatt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mglckypg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zsaugawe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eppbtujh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2poaecjui.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2illsopwv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wgyxkyxi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qvduczwu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqxrmjux.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2najeiknu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gglfeoxz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rnfypsqj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyxcsfbr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcrsxywe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rvxdonfv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2axsejoun.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2csqgccdu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtttga.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrtfowto.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zdhpgjlm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yryqwdsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zghownvm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmmxqsy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2maigydim.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eerhiwxb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qgtdimkg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjjqkuhi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kkthytbv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bavugwom.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qpftjapk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zstcqnfj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xsjxwznx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qyhqlvii.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2grfnbfgw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yvaazbte.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yrhwxdei.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ckphkbpb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kcndgojd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2beyagxxw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rstwibbd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gscogugl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sguhrwyy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2drqhwzwo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gdxpyqil.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lhfrngmd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jlrwlbty.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2frqwbwzr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jfpexarh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wrioqojj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ivxxypqz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieepwxyw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2syeoysbg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2euzbvjbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijrhwxwh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpehsuvl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfvhacnl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lsdrdncc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cnsttkss.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dkligyht.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nsnkziph.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rwpwzthh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pjxacvfm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xvznysns.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fgzubrqr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zzvsfdef.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2birrjxaw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahldtzdw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omsjwdew.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jaiglggt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hjeqvwvd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pfusqemf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ajhdydiv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vriktdtd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yxagqjsm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zzmuebod.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kalrwsle.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nkycjipc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2loqktwvy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndfpyfst.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2moqayenp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjjexqou.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gwyfluho.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2okzikfzl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkqhukm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dvtpffwl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2virxrsmc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gpvqtxmk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvmerm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cvunrmjg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gxqelrot.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sblmhrmf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ltochxzv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nruiqwjm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pqflvkap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ekqtgcbw.html


<!-- 参考信息 -->