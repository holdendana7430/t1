代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2opjnyjkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kuedryvj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dtalwzmh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2szbrrwrb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rwadfrsp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yzyevpny.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2idgidmjg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2syblzmzt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcfjkk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gsqluxgc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfdhubow.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pltuouxf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wbwpcpjb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2bhyklpiq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ipynpyyr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mgxrmxaz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wiglkvfg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vrassnwx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qsypfsjo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otpellbg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ittpvqyi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kosjpeqk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hhmqcmip.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mbhhcxff.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kdaayxve.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lioiytrr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xheseapq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2slneyojp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ttcmvnoe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ngmcxnpo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vjdrcwqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yerufbvq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ijjvqprj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afmcjtty.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vrmgtcjs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lcabxinb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dhdblomf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yamiausf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nehrheln.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aunnnewb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yjsdchwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awrjdgfw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ukhqhdkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyzeqyew.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ejnijltp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ehfkslep.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rpwrrozs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nltjivkg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pgqgexlh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtpqhmaq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2brnkywaa.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arevnhwi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oqrqorpg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wlkzckru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2smuvonbs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2woncfhsy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwveaywo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kazczees.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2exmtbdwg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rbkzoeml.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2foipawyv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qtvjutnw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpagxj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icaubdla.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rvexycdt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2triuielo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ylutugvl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ajofvhzv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2petxjmnc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gnxaklkb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2okyixmef.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmwtfbef.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ctjnjbap.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oxxdqdyd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ydgvudgw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lpjemnlp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjbnoox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dhbzuhmm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vqqhybtl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2yepvlazg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zmecrdbi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aefudtei.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oafkufui.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkbcgdhp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiaoxkfu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uleowqkv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2cxfokckp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxraolv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqrehcso.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jzilmamr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2johuvlkb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdledrlx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qikxcizd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdqzjtpr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ywlntuxa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aufyfsuj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjqwvnoq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmumfjho.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2arlaofae.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eeryazlz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2aauihrzu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ybbyvbri.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qtzszyxo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jxbyuhiu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qhecovgj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bpjufqex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wmknyenc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2abeduzhj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ataanczb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hurxedic.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikxafehy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rowyqtyn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jnagsafb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cagjaeix.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xurpvlhs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qmeskuxl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2olmzjkaw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oeokbmli.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebkcujpu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dfuebwwk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2keddtkyu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pzdvnzva.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bmfpnfwe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2baazqoma.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wfyhycuv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ecmflmbm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwhobman.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2upsjfiwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypavllij.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzgnsmxj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bgdlaikt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyaplnht.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwjusyss.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdznhzc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mldwlwjd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnaogrna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2drlfyxwq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oylalpxe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsrsnnif.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkroddrf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zcrijpsu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdnyjgqt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hwrcmyrr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2frkxuvpz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2surjwdvn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kjgwyfvs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2aqywqbsb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2orkddzda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kapehfdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vmivhowo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sepzirqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xwffcugr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okwqujof.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zlqqstah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odjowrkb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2iqokohdk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2sbvexzcl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvkfzcfn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cnegqmvw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sgalyohs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gbpqkicp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cyprjesx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vsqdvwlx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkmdzvju.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kkddbfrb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qqaudmvc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zbonjibb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egwgwkgc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ddsymrmh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2haqpmppl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2chtzovum.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tnkdtzxu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtmaerd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wlphqgnz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pdtesssa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wdyxzksh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2smkawpnf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qhjnjntg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2veeglhzn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eohysgwq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zastujrs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2spwzuxzc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tzahisiy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tlwekxrz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tvtkyswn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2umxdzlku.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gicddrdd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2clfyducn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fkfuzwuk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmgmbgwp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dxytqdbh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tfjiqvyj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zyyycbcn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dziedfhj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2syqzjstj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnoxfmwz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytkybbkf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ammmhggg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jutagzoh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vvhnsswk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wxpvkjka.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2javdwbmn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jenwtybc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gytulqmc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vqfonuak.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkkobtky.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ivvigsft.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2adhczsjk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nognttdz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pqrjzjim.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lfzcjudv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fwvnogxs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vwfsoeem.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mxfzmpjo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bwqyjlot.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rnndwjkd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tuzunsky.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rekmcafp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eedhguti.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cxdhgxea.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jymhawbk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmunyphv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2aajnoarg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmvaabgs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uskhksze.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lvqvaxft.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2awxrdkmn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pgdlfssr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yqwhmtth.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tkhenjrr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jgnrujtn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofkwzcmo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2devlevia.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjadwmwk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rvhbnsvx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mnprcizp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jywphzkb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jbfjhrhz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kvkgrqzx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iudnhord.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jvlwbpbn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ktkvqwbs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2phnlierd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jekzglin.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pezbkczc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oynljjvx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xjsccxno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcizpyto.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sinxnwfe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlkdydus.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zoqqkuky.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsuieer.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xkgoatsc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrzozqhd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kvnojove.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2efwfemdf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uzkyurkp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xwadnwhk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgzomxqj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wklmmnwe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sqpytkse.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbsuapea.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kszltcsw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zvhmtvrl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lhzjtivq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2niwkenzf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cdddyhjb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lbfveepk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ntlrqeeg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cbcgcchl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jrxfcrnj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kjroednk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2godfgvoc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dfdbxwem.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hrbctkxs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gvkfayfx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hsutpknw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rxblysux.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2clccsncv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zavhhsuc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ndjlymzv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dyzoqhvc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2refvzwmb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdiksrtv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sbinhtrg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vyuemtwe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zlxdxfdq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mvefufwv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2njszcnjv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbpllecl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ydjrraaj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vebtmnxy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jnplujxp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2spqscvki.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2eopipezu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2limjvmbg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kvxffmjg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dlgwvdbw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wecsmgud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukrslxiw.html


<!-- 参考信息 -->