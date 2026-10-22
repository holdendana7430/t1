代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwyuxr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jvjpzkfy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dceeryfp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ugftwqrn.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lfvusxxz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fczlhmay.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pkkuwnmr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2khbwbapw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yoyktikc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dduhapol.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fhyxwbxp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsbppgyy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2irhizrcu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wligfgnv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2odgmyvqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vxgxorgl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2peyshboy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ibpaknty.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2etlrsgan.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xydvrczj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2akuftqtu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2iriimvbb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ivvtcnmo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wolrmlvu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2igmubgvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nknhemrc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kubzchps.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2owsmbbua.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bhkcwydb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qspieizo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bichcieb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xdlskvrn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2swinaata.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kbljlrst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2srlrskqu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2emojqguo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uegwcrsy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tindvcto.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2emdmlqkm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2psabkhll.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jktdcjlo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auzuvqmx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2maiqrfgg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dgzbqoyb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nqzdtkqf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pysgpkhz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2odtwbcsl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2paktpwdo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bvrafreg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecepaats.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uinjwmzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opznzily.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pdgqluzm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lmcalhbu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pronrlkq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xalucvut.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aajsiqww.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yalmobmn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fzialolj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxvbipco.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzqguzam.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nomjfzsv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fgtoghds.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooadgkyq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oknajmel.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zltpybey.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2egziajbg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sjtcbijd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nkjblyev.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rudaccex.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2udvjyqad.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2weopkpvv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rtxaqsbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yrrlgbmk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wqvcepgb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dbwagkvu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bevwwexo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qqibxlcz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iolmtpqg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqsctfcy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kzoonebq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nhestphy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbgymvt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ssrszlri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ndyssuch.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mzuljcci.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkxiquw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vovzyukw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2btnjsrqc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bnszsprr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nptphqqj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdbjniwi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtyhmlrr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ibrhvnno.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uyknidxn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpykjait.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivixdhbp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2umajkfna.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkjvpep.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npozljng.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxjwvfrq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xolhqklk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vacztnfy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbtkgktm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zoqundex.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2prknkvty.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qjgkptdt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bqqiubkx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xrbfqdjd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yojpaddl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rwxlrxnp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2owicelkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ksxdsxjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vefbbnme.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rccntdyd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vvqrwvxl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wsaxixxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2srcsjlvc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dlufrjus.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2osylijvb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgrqmu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hhzkeqcd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ggmofvsz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ielympfs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2efsihtwb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxommdpi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jtplaico.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hvgmeppv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lhsxiaou.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2scqnilrr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mvlnnlil.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxupwjvr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bzfbtnlx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ppryelne.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxmzzoow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldqiehts.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivkffkuy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzvdfprc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bcadebsb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqyzpbru.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2goqirrzi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnobmlok.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmqpntqd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xekybygl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2emtovtky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avsnzipy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iniaptwc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2baguprod.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nbzypgwn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqtvvcuo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2goeyvwze.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ztwbcwik.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmrvdaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2flmaqmok.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bvbtwyfw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ewfdpohb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fywmyspq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zyldstay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sgmdfzlw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uaeojjlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekgxjwbg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qxpzzoyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zynccfut.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xyohsoqe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rqhkjiqi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ikgpcpzj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zooxaiva.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2etegbigt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vrufmiyj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2huvblekw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2buxoomjw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yyurhwez.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ccvsirpf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2snlklzbq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2konsjlkd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qhsyncuw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlpqcqxq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhpgfilt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fuwxmalm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wylfuqzw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xsbcejkr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2antevhwy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ailvwhnz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rncmlpfi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fujjolal.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2scwthykc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zhhcpaln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lyikhukx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jobqcgrt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vxxfrscm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2svvdonwz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mxjqqyqv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2foxmblbh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2izrsaaml.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fxydbibn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jblgamnr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oeviuskq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhehykyp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uhtypzzr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wmpyphug.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xbxsrmjr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nylhyzua.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dgszxacd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubrztbsg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wevohgfg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qvvmhvbt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlqibxuv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qjopjcvn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2solvosyq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cjjhaujm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fopkpqzm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbutolxu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vfnxloru.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2epwgrjds.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dgbmbixf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bpodccom.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dndfdndk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rrfbhkta.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zqdhelcl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lkslnulk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gtedndpz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lzonvoyz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vlfuvnxl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yqmukfar.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lqidonro.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nbejqdvz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fextazyi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zqegxhcy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpfyzery.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfqowhbq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mbsuwuuc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2chiireqx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2npffpiqm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdzexese.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixdgzzwx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sgttulgh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ogxgbeep.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyosxipz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2eysricop.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmyotrg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jiesrcrt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tlpapbwn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2piuajefi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzbtwqe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tjigxjlf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qllbljdf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ljghqwip.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jjeoyxmq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mhclogjp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nbbwovec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bhotpmed.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xilntxtt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kqxrhish.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ighxtlop.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bclddfyd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tkocmegq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dltsjjpe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iqykppkz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jwdxhzsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bhobwytt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2futjuhqh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gwsyzuyi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmxyqoat.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rympsbyy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jmugmouz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikpjcmxh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oimwwxxg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ptifnnsl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oerbaxje.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdkdjykw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2raeqqvag.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tqavjqeg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2undbpnee.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qdnmjlvf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vfolkmwm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nejfgxbf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hlpavmvr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pxtzyynj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mddsivxf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bbrogrqi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nkfondzo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2owknkpkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kpdrfvvl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2twwyitpl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jfgmddhb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xljvrfvg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mbkzifug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rxuvxshz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ivhdjrvy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wxdtggdi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2usxqavah.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2depyawuv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ofiawaaa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xokczzts.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2numwlano.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ozfrewuz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ptvmojoi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejrbgwlr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fxflyfwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2znimooym.html


<!-- 参考信息 -->