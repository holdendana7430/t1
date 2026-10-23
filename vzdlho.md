代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3arcjqlsw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hyhtbsec.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hpjpclqo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whyqtipt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osettwnf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rnjwvvst.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fosirlvr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgbtwxly.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qbkqqwbl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fkalntqy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcbglrzw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zomvszuv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogmozadj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oroeetbm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uijhxoup.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdblxuks.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbncxasd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otjvadck.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rrbcexyw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvdsqbu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tjuzhghj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dkgulfmm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lazghqtj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sqxrqdva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ytxxbflv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3cviovzlh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mrgrriac.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xxkqsjte.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rrcsbbnq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3beqnpuct.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfspwwah.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oeorhtao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3grlutmcy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qgsgfkbu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3oawijimj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3czvkvdyj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bqrvttwd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivebvxih.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fesfclug.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eleaowgg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jetxpdyv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hofsctmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sgegtats.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqevpgkd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rklpfrrb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uezwgwap.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrmrauce.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uuvdmgfg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxaxquwn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikxckcue.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xjejsrkb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kllinxrv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kstspuer.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbishfde.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jpmjdrsl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqgquary.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xathwxba.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwgxomwf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enwyijdr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcwonaeg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eusyvcgb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrozrwpu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mbiqlmoe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ldefrvtn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xkoerlia.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kqtylabs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hzvpprot.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pbliuhvc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vsbpbjad.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zuhnkueb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3myrjecow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bjmjhxlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sujeywcz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hqwnxiym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sssimgbu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rysfuosg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yqlnethh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyfxqkea.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hbgdxrlr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfrzwqc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfqgznjb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nvrimruc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ylvhcjhm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lazspfcn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dwkrcdcw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3syflzloz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kliwwtax.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3itqsqcso.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nebrqdos.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kbgxdjxy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bstsqgry.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hneffplq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jmuangfr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3elkqjjti.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ttkcxyvx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kyqmhbkq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dofprica.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dvscxnni.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ymgfccmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mflhfoqw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3inlttfye.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fienviql.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fbslixcd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yjjenygt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ilxutswd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gfjaihoj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uekdztdj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3btgxnyjc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jwltkkia.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3egzxpeje.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ryidykyv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bpunswoh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lefkgjgs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3smfqihcs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3teeghgxj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsouwpyn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrafilny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tefwhnpp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qiacrumo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3viaeooxr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mftfhoeh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mgzayblz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3idomfcbn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vrwhzegc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahufjnap.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3glrisvqi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fnuesqja.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kbxcypkm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vruymyoq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3irftjgzg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fxbrzvho.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xjeebaik.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kskxnerr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cudjvfje.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xysyumit.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tzbhlyvf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggasnbsd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fmyrberj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ydawokgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3usywogpo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibfshcbf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wqutchod.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3goviwqna.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrywpmpd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ttalfyan.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjgmxugk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ezayjclm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yihbdkit.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ztcmxtkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3geyyacsl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dieefkdz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcvycuj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qntiyjdv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoiexaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qhasmosh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmizojnw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zsmxqyor.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fbolqhox.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dlckcyto.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qcqznvgi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zwhllxdh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qhxloozp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zwefcuny.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hdqktrws.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fuqvbucl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gdgxrcap.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gkedwwgz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rwvfyorh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3varsqvch.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rmrsbrle.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjghoyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3viewvqkz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mexpolda.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3diponfhm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ujuxucwo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lqotrtgc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kepcdpfn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkczyini.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdsfidey.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ivgqpjot.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3inckcsga.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kttrfknz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bmflxqug.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wbkyghxj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3veukhdfo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fvtxftbl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3immqhjxh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kneyytee.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pigoislx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zlmxrubu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tgfsnfgv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3poeivbwb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hnonvefk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ujipnusk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3epycevkj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mhxjmcje.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3efudhmzj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdncxgdi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uasqvygn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xvdyhufb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gtjzvqae.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qcfwfbvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lcueaasg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiqkfzrl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zpuhmwxn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uhvsoiys.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nlllnems.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ochksgpo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tyauugty.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dylrebwo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3guemgcpq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ooijpgag.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ilxvorxc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkepxiyu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjcaiato.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kszqiige.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibjdivbr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mqjxaxlk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rbhqhkew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpphpucn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ctbffhqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfzdnnbh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ubrrqlhg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wszvgdqq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fljmxwym.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gllqanwt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfbykbmm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kpqmuizv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mlwmgura.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kaenoqma.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iinnuxic.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3uwkpbpnz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3czozklcb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ilcwyblp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvwdoeoe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwxoehfh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgyhuphp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3giawwjck.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gatfpkxp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoiryvws.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dukqynyn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jkefgpjx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lohhloze.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3edcticbk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3urljnyrn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ppwduets.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dzfwqkso.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3opuefqsd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lxqmaier.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3oednatpf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xhgrykpp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfhnbkal.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ickalwni.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fiprnmxz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdyxofuc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3axjhozti.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pjvlblox.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3olnhwtmq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3slnqtmfv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lfgsbwwt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rqcdcnqq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igxhtmgf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fllezvzi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3thlxqhhq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zffjmjzk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wmeybfja.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyfrppat.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zijhqzvf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wptsqyuj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mlnnfrkb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pfjtvava.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ygjuvhkf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oybszeaq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kpkjuond.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kbzawmfx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uldcubft.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bpqktagl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3sfhdilay.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3shxtemcb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hxrjsweg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qyttgrch.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lhzvxsza.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tvgizrau.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zjsjpoeh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gyufizqk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pcdfuxhm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xetasooi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kqyujnop.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gtkcmedb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xzqaaipi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qhbnsgnz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nryxfvna.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3skcqezmg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fweupvau.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gmawpprm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gvhlfodf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wfyjutca.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3akwfyenh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vreznwac.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ftmuakej.html


<!-- 参考信息 -->