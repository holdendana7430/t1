代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgyykcm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bnmdewjc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wyuxsvcb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eqtezzek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uipucbdm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vesupzxd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xvtcikkt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ibocagdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2njucagsj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2vcsbxltv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbnfnto.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wiwhjoml.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ndjkeeqy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hyffrpet.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgwtmiv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2auikkhic.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyicjbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rstvxfxk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kjydxrzt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qpawhjbh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hbkannpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kffnumtb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tbzwzmvr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ksuoaqqx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cokdxwib.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhrufhlo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrviojn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vvjempvc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eexqozay.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gxuyqpuy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ynaeyrnl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lbtwmwye.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2irhoyxtr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qutclmoa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ijjihnix.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fpcimbaw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zlqrlrqp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qsrwdxjq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2eomhyzlc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cybswwvu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2omsajsfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2imjctfau.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2crhnkqks.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grppunqi.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmqsmuli.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nbfqjrah.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2uyxtzmpn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ouazrgql.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fjhceiqm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vecqvhyx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hbgokcjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zvznaxcj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mgxxmyhk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2anskrahe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yywcxbar.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nljxuukv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mwvmiaot.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suefycis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cknvgzok.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lyzhpwyi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qszktkgv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rdxdbsyf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rarzaymy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2alfxxrji.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2osdgxscu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uydckdvh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2psyadksy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eobtpbox.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ptdtiuva.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rginbcco.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqdukbrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vzfzheav.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2puzktegq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gnasxzqf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fgjdpxsb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtnjaiuo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fwwnxxjd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pojosqda.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yjdyeytb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdptlfs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evhidyym.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bewnbiuw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kthbjipn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mrghwwlc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwquizh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhgkjeos.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hbtmwofj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hphfivcv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2avludkoj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2diilhdvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pjfttdvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dpasgkbl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dmbknxgc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dngvtbiy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dxqsdfxq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2prsuokcq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2znnrbmzx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yetvtlra.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qgwwczuq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jqxssnxm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2axdhmaxi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xvitixch.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgcjryp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hfailynd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwrikneu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2newqruzz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tlezqxqv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dafbfsny.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbynepyk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hrfgsocq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xynbaqxl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2muuudddi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujfrujky.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxaqhggx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awopzmer.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igzabdas.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhjtedtl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crxwuqcd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gsigimob.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzjslfmr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2meflbgkn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lynkpbdv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tcaoswvk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwypatc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2udqhlvly.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ljaiynxx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ruvjugad.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hldygvzq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wevkbtqe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ducvfjmv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xzmhofnq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdygezmk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qykvwxlp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xoexjjbw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mikbbypv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kzkxurhl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uwowkhqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2atpeoiwi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rfxaruzy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkemkyu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rvbjbrwa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oeapjwqq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unpllauf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ivdgihox.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gjlinrjf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pgzbsmij.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mzhxuryo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehrgbhxk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rbgonfaj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ppovkvjb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjimliag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxwufwhg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vioqkpac.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tewgsfrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2aqbzhfoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovmsfyjr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2twlyizbq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kedytsef.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bgmeocjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syhjajfk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iqfzriwa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rblmyzqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwkzkvkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsxzakmz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nctetpzm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxplvlmd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgcuhjd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mhkiucvv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyosecn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nzfiyuns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uoersdpp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jromkepl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ccsjnpox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2grilrijd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jxfayfxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rcxohfju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fplrlyer.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qyldmmqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwdfnnrk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bfmlulga.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2khpyyxqp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2geudrzfp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lrkdrpoc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxuvlbcc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmbmhvry.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nosptgel.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fbowregv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxispvqe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rndiwuer.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dauygpar.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gmmwqkcw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jfvgfxnw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mvyxmbms.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvdkbomk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jmombofb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwcxandv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2edojpkbf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2apxwyomx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2drvlrzio.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2khzsukfv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fzwwqeio.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hqamddoj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2sdoylydo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hzdavems.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sfiynsah.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ntmeyvjp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oarggceh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xzssbczs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fvnlydhw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrcnbt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xupigfrf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yozffkfi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iboqnsli.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uatrnkvu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcpbgpm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ufmcbnbo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mhcgslgq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2edppzjnc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2amjfecic.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hvnrltwm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2avczmqim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jjblfkuc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2afytpaqm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rmcccvcz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2owmklbhr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rjlbqhwt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvbaeptf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhblikqw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chfwgmgh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnwslawp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tictjcxy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2icpqvyof.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lomkodhq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fodzknpa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zgrxutix.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hjrthnrr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yzdtmnjn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yhhnhatp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xssuhpbm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hcygjqhg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mpvsqquj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nuvkfcza.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pcmqqnyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pxmygrrz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggcxomdt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iilbtdmc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbeholeb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hohmlecb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vxvgtazr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rzyznvcu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2diubzslr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kqdsiyqs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fmlyapfl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdgdkfrv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wmjsfvij.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vxxlndmu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgiesnli.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iomslfho.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwttobts.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljbfhkap.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2paywnntf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2deblzqst.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nswygdts.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ayxaeloy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pxsgddxj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2llyzuelo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kyhbzupt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oyhlknjy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bjqrjrse.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ikffnpar.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rtqnonub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itqbgbcl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2adysiany.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsbzjst.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swdxmlnx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zrfexhgd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fpeapxdu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvfuxiz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lcpgmzkz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vodtjbar.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcuqyfj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2prabwoxh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwwdksrc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lizfpdvh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bufrbdqk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lbuvnazq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hgxvzwgv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bncznirl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fumdjpao.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kcwbvxlf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2extmdtsq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urzbazep.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vpgqczmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ddgpwkho.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hfxdzrma.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ygcscimh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qkvwznsn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pvhsbdxt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jtxxjcck.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2eliowmvb.html


<!-- 参考信息 -->