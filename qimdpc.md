代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2smkizzyq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gkkrunsq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yiwfyhcz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ugkniyhx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hshytfwg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdbuia.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jurrtmzd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoutxed.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ehdarqme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hwxdhtfq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lexgdyye.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bphvedeq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2svwbuoay.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhivfwak.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gygzmdge.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rtajitmf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rcdqhvbd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qszjgkzw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ouwlttar.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mehglfsp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gvpbhwoh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2nrsevrrw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2etwxmctd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2opjeeztt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hnxltnpy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2urhkagxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mtjnxehy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2rrxetykq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xkfrtrya.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ctbmctbd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2stehpqjj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqssmxmv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xnqhatss.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2adictjok.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2whgctbcn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bmsspaoh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ldxfouap.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2owcypwee.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nqpkmlub.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2rqtwlyjg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fphfemex.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rhbsxzaa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2umfbbapz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gjyylxmg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2chqkxkjc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ibwgifub.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hhgixthr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bspvxqtq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2aidhndmr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bjsxiuha.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2downylss.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ulmxpkjf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gbbmvzgq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dpdjaxwz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xiipsxux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sqrzpmey.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xbtlxeft.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dqpuuwac.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mfsgwyzd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bugryddw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2giqziesz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lxpmhfrf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hvzvpuef.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ggdplkdv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2upodognl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srivgrrq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qxyaoqow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmcbnbmj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yawrsrht.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kyauldlx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vnkfgckm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wqdufrwx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tumfusuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qgiorofw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2otwrhvuz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gamdzmmg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nuhrkpno.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2veytmwnz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xugnnhpn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mlnwfkvn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uqplbzdv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtsrrvgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hnfmqlmx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qanuwitw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pwvhkzjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fozpwbwb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2trijiocn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ewujvmyn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lodbouww.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2woadnaph.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2letrdeza.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mdioqysi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kicrkock.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2waxpebfx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dplidacx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfywxsqc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqywcdyd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mkkbixhp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lfsrsryn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pcgbvwzo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qaargqfd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zlenyrpw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxhhocl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2haklhktt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ufpfswim.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vxbnohff.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hbfdtuag.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywjypnew.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skxplrjj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbfwkuvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2racmjxcs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bajdacwt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkmwxhom.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rcbeaykf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjrbpys.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqlsjexg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mszvyvmp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffvfpeey.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhiuidce.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2onyllbdt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrtxqk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhyqavtp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bfzgbrsd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ruouwnng.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uaepxyli.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zgbjtmlm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eznjcdol.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vziqoxbz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sgypekoj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2prhowkdm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zdhlhayb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dzjbkabk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sgioowlh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ulalpplm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrltrspo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bgdvxlri.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wrpfvmsg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wsoybyac.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uywtnmfe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mpgphhlh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fiytolll.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khepmnqu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qucjdlzg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jgpztrsj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tlibbmpx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzqssa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2szpdmvrj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnptdvhx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uvdkigzu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2faaknmgc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bokhccdn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hzopxwjj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vblbiaoi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvmwwmis.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qtxygfml.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aosidcdh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2breedimq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2poebpqgm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hpecqzuw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmhucti.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zosncdqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weuidgeu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sktoljrw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wuwqnimp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2maciylxc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bncvnlwl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vrwqqltk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uktwrvlo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lehcdcuq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jlfnyfgb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jcwminfx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dtjladwr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qzngnvmi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2thitjemr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gtxzelhu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mqadlzyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lclaserv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fozqpuvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsszneol.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mdzpqzyq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2avxadztm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2auaayycz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hkzgdhmw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqvaffte.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2spedcvvd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ulinagzs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxdhipdq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gtakmizh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gopikcvp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wilkmdes.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fdshlsym.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2plagoudd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiwpfpvs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htkwmhjx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2exscktqb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2apykbjcb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofdvlkn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yffgxuha.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fygejhvw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfnehpvg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yhrcyuic.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qqmlnhbf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pdpehrgd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ixoklzvm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gjqmdoek.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2emnszmio.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2eldhqvpf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xtxxjrug.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gqvhbyqm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fhzqdrgk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ukgujuax.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzinwyhx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kperyolh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlymkhbu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ouhggcan.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qywxirds.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uyjtnmrv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhqjulcj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gjzzplci.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcdanxfs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dtmkaqpg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pkqtmsry.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vozbswee.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fdwyackd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yqlcysnr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2upoejflm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hculkums.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2soegngtd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrojxnuy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mufjjtqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2djqexbjn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ybodivcy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uzwndauf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wcyxknqz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2chxahztl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ymjjlpes.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2limcisab.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wlpxorol.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xgchodbx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lrxrlvhb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2buerkjck.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gciexonf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tefteavg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jcmkmwot.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjgqlvtn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hufoyhfc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yravxjyn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtpyoheo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2eftvagzu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnlhpktk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jgqejutp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2koztcrps.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fcyodhev.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfmslith.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nhrjvkyj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hptmsujs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vxximeax.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dcyozgdm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcwqwfxl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rurjzbvr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hwbxvlgd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fbghfahf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pgwcslxm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jjowqion.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wdfwrfqn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pranyyxk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zjyvovew.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sfzncvah.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jgdgcvpx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rnmepryi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dmaxhjke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fvmichqq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iclceism.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljqsxttp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2flfpyjqd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nspahwpg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zglxnwiz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ydripwhs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dgmnfniy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qspjhgps.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zdlvqprw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aagagull.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ektduvxt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vtmneuid.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ecbnqkko.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nfcauqku.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nsjkhnct.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lhoymzin.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2busgixxg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2akycvxcc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xlmsoudg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2exyqurtb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lrbnjxpc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2iozvbxhu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zpewmzwh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ovngpfmz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vwbkjmvs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hxicunxl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2felcuxag.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2phwjyndr.html


<!-- 参考信息 -->