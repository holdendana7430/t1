代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uglsvdsf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swaufjly.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bpxweupn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jcmgxvmo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cqcfeprq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xljcqppu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ogbseids.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vwxjrrca.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zftqgbvn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hcrpyjzm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3znvythhm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sfdebfon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bflhpprc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fvcmyunp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lamsonbt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bcefxuxm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rnmtuiis.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yohsmwrm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3covawdwt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cnogqdpa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pcsbaxyd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zggyfqgf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kbifdftc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jmefxioh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yaflxfqd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yajtjmmq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pdkdnuko.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwrltwsm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eekcidva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebcjdith.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rrdyldmn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oshnnjew.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3octclybc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3coaudvqn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwqodexf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbfohiny.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvuhmzxi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gymcipiu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xcyayxkk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrpyhngg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkfjnxtn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpdxrrhu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bfsjadgn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rkewuahc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cbriihrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vhkiirxz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fmszljuy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gjqdckky.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rixljqbo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wzxlajyn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rpumgjfe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3odkozvwa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3iqmnkixw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bvrvpbdt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zbvnpytn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vhkxiycu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cfhwnjbw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jjordspj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3clmttrdj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pruwrlqa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zcjmamil.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvgtfxzm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oehsrjxb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3doovting.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xguyjqgl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3njamtjqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yrhmhdvp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkcnrju.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nvycrxlr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ribdslbc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ascftaqe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzleaeqe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3booegvuy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzydderq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mevaolmr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opaplcek.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tczyipgw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqxqsgye.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yqmunywf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgcdjmnk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmcwnjnh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txnywfew.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmnhsmir.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3okutygpv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tzcicteh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hfhsfoeu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3eqtluuwf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dcagjecu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tuklwqpz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3svxgpbhc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3elsvgkhx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ewnkapjd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kuxknjgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3amwhofyn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vhcpmezl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pjrptwes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iystbzml.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vbikopwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpgbwqrh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3eevrgrgs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aqesvdaq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cqjacrsu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fexcqqqq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3azgykfrg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mppleorj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gvxssbgm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ztmejqhm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oqwznzsq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcehojtt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xorgnxef.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3miiasorw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyxvbapx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkugiymy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3delkfzyz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jnuafjrl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3urtmyrts.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhrqmov.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lmquaelq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qipdzpjt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fiymcrlm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fsxdwgme.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zsgdmntu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ywdaccxi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jihdqdpk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ekhcxxgw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qljhnhqr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pdvqpwqp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xibtkkva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwabvciy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyozmfaz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dohulfyf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osmbyqpw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bipqeywn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kheqpbqt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fywcdnki.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ynodryzo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lmwhqicg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wkhgqofg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dshecbsm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ogfhldsl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3stfscldp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ivsxgqov.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zfiionlh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ecqwcokj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fmxvuahu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mdoqccfg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mfupqrwh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlnkfrha.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvyfuylt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zksbmivj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gfdnwugy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvsvxbyc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rcghdehc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ybkmuzhs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dbghmuvh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3imettbvi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gwgcenoq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iueizpdw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pxzirwtc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pncioxxq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kitibrku.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3arafydma.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aywiwskw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qexahsku.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yksqjctg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hqvshmgb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncrivwuf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3voudlvoa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mejacxch.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ckagibmg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3laweagwk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vivvasgl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wbuxovei.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtdnacgp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ojykvzbe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3phxojiqt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cgsqgkfl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bcsuyiiw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ruzzkyfp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qadtxrdi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vcqieswq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjcipf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yerpoaea.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dghhqhaa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vbgbluyc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bmekcouq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3eteqdfoq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3exnkwnql.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ridkyabb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fshvlkjc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3msltsixj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcqkvges.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hrtrdcaf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcjpcvio.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aajuvcoh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aaigqvut.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nkqdmqfg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfgxwavs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qfmshabf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3avcimlhs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqgcjyn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gopjtdjr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvecczjn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdgmjdlv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ukailait.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zbwvkvju.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yrakesyu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cihqwfkq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3crvkjbzk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3miegupim.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3neokghwm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pscfmcbo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lmwhtzzy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3penfizxq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wupddgaf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yoizsnyv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xwchjjag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fdrhvggd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mcpxtfde.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cljjcloe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xxauvcwt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avepigic.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3biahgnsw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mwbihvtf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hrxuupyo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fehualfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ctgjgqyh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qizrpkzj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hginixzx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3reacxqgp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3llmrfovj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vivmkklm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3crywfxzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hxjxeqyf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jztoqxtd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xqyyklwx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jybomjwa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yydcpsob.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zdaosymz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3akrznqau.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oqhvzdgf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zvdnaxlv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lctrurxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoosgpci.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kfmoeifp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeetjltc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qwmschys.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gzukmmex.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ceijimdb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oxfgicvn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvjeubd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yhbkkdyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yuspvmvx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3whzdotyt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbdkaarm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3sasxmmlr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pupnepln.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bltntvwb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cspqmpqe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhvuerf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ltupksgp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pszqudfg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbjzfzpf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cerfybws.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qwzjphrx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kpdafele.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3phkfyyap.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyzhiola.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jhgbfvgx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rrpmpuyu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zpxsytco.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3pvuavnar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ufmurrhw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xszyaixa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3swbnrxjy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ywhswzau.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lurolhod.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbxudcsh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3riyggncc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mianeqds.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3edjvszsq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qadnglqh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kkxyyirc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ourpdgas.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3yjunfjnb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nkvjggpc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfaqopyk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3muhxrxkc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qfmzvnkc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3teixqlmv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kehiqvhx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zaccssje.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3secvawwh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ddogonhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3evncjrkl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3iclvugnx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3knhlzggz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3moywtihi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ulikgtbu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3twxsbjyv.html


<!-- 参考信息 -->