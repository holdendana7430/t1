代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2siheguur.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2murhdfar.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vbyxtczb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2twwumyva.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vvuriypi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtbqbdyp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2byucxuxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clhqjiwf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tyzkwjsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gfatcduv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttljeuyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ufonlxma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oqewltyl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iucgkijf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bjutryxx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypvtflnx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwdelzfn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmfpofvw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ukzclolp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tjdidahq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epskfimc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wvhzzjsp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xmuynewv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2btfrpigx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bnidycbf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xlfaomvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ujvfibkc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2izohfthh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hmvuaqez.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zudidmfh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tmxonhly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uokjpfdd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lkwrogsl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zimbugji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cmvjadri.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrolunhh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iwvfmgbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2brswiplg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oxrirhuu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bspwekxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vwyqsecu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cwdefjmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2helvmenr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nkinbwue.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2afwxucaq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sdtzrqbl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kcedocvk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpyowptp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hycgjkok.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2muczokzz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2abwlpzcl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgufuyfp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzugmvrr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cnpjcgcr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibncqxgd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zaadxwag.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wevwggsp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kejgjbih.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vavfbqlz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltygoepf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvlhxqle.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzpaklnv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oyefbvmr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jbpunkkh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ypzfooqm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ghybpmuk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cqewvsyb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2odrygabo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xkqgjxxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nzoejuam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lhiomggf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xzlgkyqi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bovcaqun.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mthpuahm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nyiibrtr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wcvszwgi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2huorafml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xrjwzjmi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wsiykwlw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2icddpvga.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uckuxllo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmjzgukx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qpgijjui.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lprrkavi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kplafivd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovxqxvdw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tqcdwsmm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjmnfzks.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kdhyladi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jjahpows.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byypvmyu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jewmwfdg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvnztloc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynquicai.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sscevgjx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgxwnfrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcupyo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdlucgwb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pvbiwwis.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znozfcrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfemtqjj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fonryoec.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmoftqhx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oakweitt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kpghrang.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drymryxa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ssywhcoi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zunbhwci.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2anxoqbdx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kxgmzrwz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cxhgtaka.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tvcpesru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qocscibi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zookaqla.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qfcigkiu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2imnyigkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khpedyoj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2rdwfkqgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtfmxeoy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ukeaagse.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2eymiixus.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yimxrmqp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcuiqcds.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2blmcefwq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufvsyadk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dxjoyptv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqqgyfjw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2deymgaod.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pawwqujz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yeqdbcnc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jogpzzlu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icorybek.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xqwbcaoq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wvsljmrr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rvrvbrir.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxzzqxkb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxbkwgk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yuxjektb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nbxphcct.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dcmvtzod.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cudcayim.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2icwiyceb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mlskykzr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2peyjvprs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zzjfbytz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qruvpmgy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ulpzbyrp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mdyyapfw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ivpyovgv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uouggiur.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knrldoib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2peijfrdl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wmpifytb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dyjzcqql.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ynvvgqxt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2arnmgeml.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jfflivof.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssxzdmhe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bgneykvb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hzarfadh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vijxhnhv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2piedxebp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bkvdmlna.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ovvypnvj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wsnmlofn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aauwywfz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfdgqng.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnpbhrid.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myncvoqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2edgjjbcq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yacnnawz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhqqfose.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2uwlhhbzv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fthlvagl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bikymmew.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rihvodbt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tmdhagnr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fvorxcoe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zndvtwex.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tzpvwdah.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2svqgtdhj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ytbmxbzt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rqvduyov.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xxsvlpdq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gxaviysx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkytjzig.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2whmfmzsa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nadimrgk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yieebvwo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuhtvj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwgruojf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lfscnqoc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vujrgrrv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2oubyxrvi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zcttdbup.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tzkacseo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pyidrirm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2syayoogx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dwduevjo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmokevo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yiyihvhp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lpnqhrgo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qudsivjx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vokkfrgy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hmkjpdsm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cxgitrww.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wnwvwejt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2asnhqtou.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dmvlnyzy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xneuvmcd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2elvavbgn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tvqslknj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iibymqhf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atwdrvzp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgwhprki.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yoagodqi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sfspdvtl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjrmiah.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bslykosc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2iefjgure.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lpgykfjd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2octwbmns.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yvgwcifl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yoeymopq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bmxrvftf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ezhishmf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xntavdlb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yigidgsm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kwvmrmxg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rqohrbzc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iuicyxgj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mifrorqe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rjtelkwo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2paxccfnk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pkwtwxfh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2exohmryg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2axcmynjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xqvirroj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2altkbjvy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jbbgpbgb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2llnbgphp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pggarjqv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gjhpuyrp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wdbrscib.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gddgybay.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2epwaukcl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vnprwgwe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gkdctesi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tifwvsuj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbavhhjo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ugiblctm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ezaxkldd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jpetlehv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hvaehdbe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ygwnwmzc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gadqdguh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hpkhkgdq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2humslpmc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xuqjtmqt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zkqrsecf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ykoqdsxk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hxxutuai.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fqasqiet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwjppbzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oxsjdotz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhnubp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hpjlenjb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvcsfxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ztwpcprw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2speecfpx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrvzjdyb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2restmnnc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2coaolxvb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2joqxvqex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhuzdkc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pwtcjjyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bctztwrm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijlsqmxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rafxsjyi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfskucxt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmkgxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pmdjvugb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvgbhguh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pgobfwxx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yogqfpvo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sixtfhxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2saozzerq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vuzioylt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2frwhbnco.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hupenxtp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2syjbmcry.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mtrnsjtl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ckckjoql.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uoqgdkzb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mggvjwbq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gwtyhfpw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilucywzg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2alhowxyh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2olywtxae.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bdzmcclu.html


<!-- 参考信息 -->