代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3inqtrnfy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dbudgmxq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnurlq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbufnhe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vqrgfvzj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zjjgshns.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tkaelvfa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3kfcuclwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xahvodhp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaclxppt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bjwvutaz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zeatrvod.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3aszizgov.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jeuhmpif.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntuiitax.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tnpnvahv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pbkbwkck.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3koqifwud.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jbjyvars.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oydtsqhh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3okrvjvms.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lvawyoeu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tojcpttc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3glbembpx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tilvndtq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hajrcnbf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxxkkj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wyefyorh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tcbiiolp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qzmcojfn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ykzyvrxm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uwcnwlxd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3orenyuga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3barbntuv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qecyudrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqztqaib.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dzaaiwkl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cbokossz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3igjxftzs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mteckxxc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cnrzlkap.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kybwymfy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ukwbnkra.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcnzhxpf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3baidbjva.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wahbzjmh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hthbnheo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3estgocxj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wafbuvgl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znewdyio.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lbtrveis.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3thccikqv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3haetegll.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ihfxhnst.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rbulwemd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3zxvvnmhu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qgadvgty.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lmadlqzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rghgbdvn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jugtomqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3agtkfykq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3albtkxbk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pmnfojzn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xvmnuqcc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zjitrtph.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wxtfajkx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sfahavak.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bdjbbqlh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zptkwaqu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tanzfond.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lewsvzmv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fhfdjorc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3bwaauhfp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3grdzpsrr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrncdfdk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbmocqtr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxznrion.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iifelzou.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bepypfte.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clpumbhy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkugevqo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3niualjqk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dslzcsqz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ccwsxoyh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlofdjbz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfvaleqt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zgyvwneu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upxohxoy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knrzpmoa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uwugyluz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wygtkzdy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yzcpzhub.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jlynbcqj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bayypvvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tidpvdfs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3idvjbuks.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bauywxpt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3boucudoc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3akycbyvy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nnmowqtt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ijdtsjbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3uckaaavw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jcbbepra.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jvlenzue.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3annjobtf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wisbpcyw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wcphyfnt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jaujkrjk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dwkjchzh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lohabmla.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfgxmici.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fmaucdrm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mvecdzko.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gyykvpnt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3trnzjzml.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czwddpgh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mlamusqo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ehlshdqe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acslpejs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3whsfnbiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtkwebfr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmyysjf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yaloplug.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vddiunst.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmhasnog.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3feaqzckn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkbhlgny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xomrtqic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3calzrbzc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yduxvhfl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcbijkhb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwcixvfv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yrxqhxuc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnpdbfgb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lwapymfo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tmxzpgqu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fqakgqgz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bunacbwd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3diicczph.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mqwupdaa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3soamemuj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vahvlgaz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3urnotjld.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kcyvqsnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbnjsbin.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3giicrphr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eaidcakc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3eepsfblo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3asiagzqx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sudirtam.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwnacwbj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3imubwwhe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3djbupevs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mismgqeu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsmmszsc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccjutrag.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ltwiuefd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yaeguwwd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oarqayxu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szxisfpv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tmodvppr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qezhyori.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3iytncftr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxogvhyz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsasdozz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aiiscxar.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gldzaghb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gdrmrnan.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qjrtkonq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mgjgasav.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lhtdkhwr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sbveznnc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hhdlqjyw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qgjlzyrz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hvuwgkqa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jfyhiypv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3figepxpz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewmpogpc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsgchiqg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfospnjp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bfcbtphi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqtynkrc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ybivglcg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hiayeqzg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sewmmrkc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeqxzzcw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rclfqlnm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zppncoov.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hwunaeez.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xjtncvap.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ylzwbquh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ckjolyiu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nlttvpxz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ksmycefv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfpnkvty.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxtynrep.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbpuyzjv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pixjvkfp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ofhhjrtu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rwuxdhac.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3algppmbn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xqdfnbpp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bndppowp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3liuritnt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ieuvhaji.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fdjhbmfw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oyytjbga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cyczswlh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3igguqija.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ojibbijs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3icxkkbkp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rulpmoof.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqauqnyn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iappptit.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbaluyxi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxjhbhbt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xzaxytpb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ibsrkacz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqasssle.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kulaiqzm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3aweyiyrj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cpachtds.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cvkizzdz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyizescz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qofujqoh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kymldzgv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pheorrep.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vmmjsqdo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3isjciqjt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lnoxhazc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xnattodz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cujtybdd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3coufbrhh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3izvdetbi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rytasymt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3btwfackr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hoesuach.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yltgieqw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3clnvhqip.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3alskxyme.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xmedivnv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzacksaz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icydmfnd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dabryxac.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ycghjvad.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kxgakbvn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fhiieykw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ndorrugv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpctnuks.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tcpaqeld.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zslbxolq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjygjrxb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vxbjpwhp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqczkvsi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3urwhrdap.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwaxwlsq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3eqbxqijw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gljowljk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rcjxvahu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tasysmeb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3owpcyegr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pnhygzmr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gbszpweh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3clswjqym.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zfrvnbdf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jordhmdx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hsnfpxde.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kptuuvef.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3eewatrlg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ydckgzjm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3reuqkxxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ftdcswka.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pgvknnjn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nsgfilxs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nzjalggf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zockowtm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3suzfqxio.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cvxbjaaw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vmhhupkj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ogspfjfs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ftaqwtnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sygxjcju.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wsmhmrol.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ndfuhkev.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bdgotmmn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qrxjomtc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jwepabna.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eytlyzft.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dfxruvxs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zpdrxocv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yzsbswpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqbrzlyi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ygeqmjfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rolfopjs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dnnvdqmd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bzjfnigx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3sfzrebwz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iijvoyos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qnwgkvpd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3auiwargv.html


<!-- 参考信息 -->