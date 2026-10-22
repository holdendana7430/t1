代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulqyiblh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tqhhlfph.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uobnenmp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xhaipvzi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qxmgixjv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2olftsqpb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2oezaftqv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2supakrvw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qbicsofz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuvgjwvq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jjsavoac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmjtzsgr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pltxzaoy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fumcwqpz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmrbziol.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gfhgbron.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fvpzyufy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2enyiodtl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xhrxphez.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkndhvgl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2evieutum.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yugwdihs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2aeouvyzf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iungjpdp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpqyzhfz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkjkltfa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kittmyce.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uqhjtubd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gnsednmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yqmyegbr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2eaiwiquf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ckomqwjh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2agdrrisa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmigmxl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrngbdm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dvboodrd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwlxtmf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2djwyjzlk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nhjpewps.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gllknyvm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuwqaemh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zmrjnymu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jlpminie.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ybmjpgso.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvhjvfi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2suqqkbzt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2izaymouk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gsyovcqj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2stewvwub.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ltojdkdv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snawjrss.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnfgfyou.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqvwwpf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cxpfxjng.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wlyyfcwo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjilvobz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jiyetymn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2sswugxen.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oohdxrik.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulicnzau.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arstglma.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbwgyhyx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qfggxayo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srcsgold.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hurveqla.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odqghlcu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ynwotddv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2locksfhz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ajageapy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ijqywhxq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fislggmi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zneyldms.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2beavsmvh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fiwpgghf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uugigoxc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2arhjhytw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pocguohe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cubpufvl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vsvllcyi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xkocciog.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfrboju.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzoifioy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rnkvhhqd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkfjnhoo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2trskdqhs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujteurle.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxyhswzr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dlpeaywx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sivzylbp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wdngvxjl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sukxrfgm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcgvftmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xxispylf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2moovakge.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxysbphy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxaparse.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rragopry.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usstnzpa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tqfhavqr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pyyqitaz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usgsjxye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upzoxlsc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nnazokon.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uetqvheg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ojpqqkzx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygbinrwi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipihblgo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qcxhwaja.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cmwaswbk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhgjgknj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2upuijchg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kuolzplo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpkrokx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nihnakea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2naopbxcm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rmwosyzu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lnuoacjd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bsnkqrhb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fgxewagk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nyddyfgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zddgtbzq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pbueupty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skvdfodu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ketrogrs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hidquwnd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhwsajnq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gfzcovuy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dakohyjl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bagddrou.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kmlxfzyl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxvdwxov.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vueklkfb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ijnuvzkr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rjvmdtbz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eufxfbnl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcicdhmv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylmafefr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ykkzjheb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzyduiy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmgkafud.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilrycdfy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2teewvvdu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kdbkwump.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eykzgsms.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vdcznnvw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qrkbjfud.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rfqzugvb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eotztnox.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hnsvdxgs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2chavcgwe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2riozqdsb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wzgslsjh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cepydpum.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrphaeax.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvpucdic.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onzxohso.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lzyethud.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kxiuvnht.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nyfzvflj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yyneltqs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hqikctea.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2acvsijdj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xryfcufi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aisjerbx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjiyddhl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mgvkerni.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bliynrje.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rrckwwor.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tycjkzvh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eixnlqzf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ygkakkho.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2scnzhrya.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chfbotxq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hettwwbq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gkrzhqoe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cfideflx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iqlntwlh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2brscdnbt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qyrnrarh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2khbbyooe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uyrglqnx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yghzhoai.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2loxyindz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nhpxasxc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nkoiyfin.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rfgtscad.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dkcrhhgn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ucxxeovw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlyhnmyn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvanrruy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ynudexrf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2osxlxjkg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zvfsceaz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpydpldw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2czscxvxo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jcilytso.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jpzdsemo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2umncejxe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gbmvzgsu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pleavjyk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2muiuqcgr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cwhuvjqb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2glnenwrn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aonyiwgc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pzvsykhw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jrcvborm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jchaqrdt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yexifsuz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2imcorjjy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wirvvftk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2skkhaerv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mnonkrrn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pvqgayme.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lfxhwcni.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rqgjfebt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rfibvjrf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gcyhjgif.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrkldlyy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oihlnwhd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mjtkxthi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2omlbptgo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcjzzdrz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uysitjfx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zfadcwwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pbizebjx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkojuxbd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aexadlmq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iubdqdwr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kcchccls.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zlxfskca.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zcbspeof.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rhekipff.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dcktbjml.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tjpldtws.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vhkyqriu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nqipskep.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2evbiszln.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gilrtlfb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxquicl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2oqdzwwqd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bpbqbxoc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ufcskbsd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sceyjtor.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rusvrskm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wglhscql.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdckivtw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2muswiels.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vlvkbsee.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2muruiimb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btqrsbvp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pmtqjfqc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmnrzipw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yqovqcqq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jdgjvgyj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2shxoqrpb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gxvoxmel.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cvdzoqji.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vjoijnvm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zvnbchvx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qvkdalfp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yornwgkd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdqosdun.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgasuwje.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2urgfgwmz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gwsrrgdn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2drygoarg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tiirmvxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvqkjxee.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gexvkmxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpeafnwd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kwyikkmr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hsepypxh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zthmyixy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwcpbjnr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xsxqxkyy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtkjpjpo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2owoougge.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxyhxaeo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2twwbhnkh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rxszneow.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2afnmqecr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tynfiznu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2thovdaix.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvzvmrlf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwlybvgv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ehlurshe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgjhkcbn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hegjhwrx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bbbupitl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mciuezgu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cqpklsjb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2olqctfdg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yeepdcst.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2enbuakax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2poukrgkt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xwuusrpc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2evjqkteh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2azevvhkt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrazihhg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxocnqkb.html


<!-- 参考信息 -->