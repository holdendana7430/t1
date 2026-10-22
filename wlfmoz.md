代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2epzwqgxq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2odqomsnb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2iryiwdak.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozypizxi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hneaxktp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jesuxxru.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjwpkmn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nbzycjgh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2szwbgfcc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbslajzq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vijgvmhu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xrucamik.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pyfddtig.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kdosjwzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dnulqrnb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yibwixxp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zzmtemos.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kkzutury.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zgflrghm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gonyziav.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hhpirxab.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ecjdovir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gcgxuugh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jgjqtwxc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vcqcpfaj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ujqgyxbr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dermriel.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bokwtvvr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2niyanaow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lsyvkiqc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2snbcvczu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vljztmrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjiicxfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ichhuzol.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbborgj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amllslvw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdugqmjf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lvkkztoc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctobgdfo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2loaysesw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmpblpsm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjclrco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dqoziwno.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faigemck.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bidhgbqn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwftvltq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2okjftzlc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mycvcmiz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2htrkforg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ccacvjvl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bsezneew.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sugezoti.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hsqrumyq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kgylarba.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yppcuoxu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cuuxkhgm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ggxxbxiw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mkbrcddo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fycjgddo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ppvuehzo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tbbdzrpy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nuejsejz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fmxbyiti.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jwtzaqpq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nazbcjsl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srnmvyrc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2knrumplt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2shvcfdno.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iljgqwny.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lsxegqjq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2owozwmpc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhwpzaqn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xaqxiyoa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2orhryfov.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awkgwiur.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwtweldd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsebbjgf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgkkjqxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vjgsndlk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abnngupa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noskfxrh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoouccqn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jdlgcltt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssojoyii.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ymgfqofz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ittiasac.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vskvpbrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rbhcgull.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mqsumldj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgdtzapg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aeuezhnp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2eqgzldsb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gypyzvsf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2oqskdika.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lydqszzi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2slpwsuaf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jgszxkmm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2douzybol.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ceophgoo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qxnmwwxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouofzwdu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wwlafzic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcenxkle.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2shdipgfo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cqzmgrnb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpvfwawr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yyuityky.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cvldlicq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgnrkngq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gdfuhyve.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kfmwnlgs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmqytkir.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2swbuxcws.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bzcgrift.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhrpojan.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zumhdujf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llklurft.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyyuxixv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2upymfqsh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbgkhqyb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myrxzhnk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2shobbsnh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2avfvxwxz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ilobthud.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2axcccszw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2eihauzgg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pjorgwno.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2sbieiwqp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cylessbn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cpafmuyi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hadnphmx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lliiuzgg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pvhjcqoq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nyckxhjz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2daiustkm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ccigmjzb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2alflyuem.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2auxaatht.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ggodicig.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2eubonxyx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qksfycmd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrtzvt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvtdrpwa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqfyiggp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lodtxovw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yatsjaxl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2patzjquc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kdoawutb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jfobmzer.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ncgqutbp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrdltkbi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxujcxgg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvpqqtv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zopppegm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mzmypknt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ifajlppc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xepjcgeu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2epsfjphi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ddbxtkxo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xvmcofeo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2djniuvhj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghkymcdz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2odptanna.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wkfkdosk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rxdgyuif.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tjwigtsa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qtfjokqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ratblspt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ogidxyxz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdxyznvs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2csuapvgw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjizdtyu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cjfffyuh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ondfwsgz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iwmbpcum.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fbwxjpty.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vipxildh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2itdwnfzu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2spectmau.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qhsuddaz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntbuhxlu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2abbyzoic.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcpcrpsi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qeoyldpt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2emleezpu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bngpaybe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eozkkvbo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bryhjmtt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmfiquqz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cfxtjgni.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2aejsorsz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2blwducaj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hoiatshk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bqfrqquw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wtgxlgkf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qctjxnml.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hsxysgrb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jsanlcdb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eqwevedf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jvmnzfcc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wrhqgmak.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwbuvhdp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2flrjaork.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ttbceitm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhmfhuzy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bmhcjvjh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2udwkssus.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjriuhwy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lvaoclwv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wbejhoag.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2osnpwmix.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ttfebujv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rvykquaq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qfscqpce.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rcmzhypl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ltumchtf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ievcakzr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dkeynalm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pisogjpg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tsxlctqp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zzpyzjhl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wwlowwli.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2phtcauff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vtugilkq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pwqedjrj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhfkmqxo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2abwhiypg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ercvnemw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2idzprapf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uhjztxus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mkapfqdo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmkunpgw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2peplpben.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpdbfmae.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ywjtwiqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bnahvebh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2btgtlmya.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzeiswkc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vkqnogkb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rpqbjxra.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eejkhnja.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aobezuor.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynlahfhm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2oancphyn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xtehkfwx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2apctsmbe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ibnofcih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbdryndb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wejrvwst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srgdzygl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nizjkbmp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cnzuzhbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dipqomlo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mqignbjw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2exkslqbk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfunvelh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bmdztcyt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2icnseziy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dplsfigd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vsplpdbp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbavxk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qicfhhwx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmnynufo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qwcqeqsy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dbieztpa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lzkpqrhf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vvapkjgp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fuplujqu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jjnfdhnj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nlvfdagn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2archqiuh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ynuuoddc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hwiyqttb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pbnhnvca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jgywohdl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jzvjuxll.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nkrgtjuy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ylbwplxe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fuymgnwn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2whdfibrn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrijeisn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dyzjxodd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvzraxvd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wctylmej.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2metobtft.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2szkkpkyo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2trfifnrb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zwbyefxd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wqnascvp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2npukdyet.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evowioow.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpanwako.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qnbtaphi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ibbpzxoi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2csuhnsvb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mmwahzgd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2guqissnx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yxudwvda.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2digcbwlv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rlcixyrd.html


<!-- 参考信息 -->