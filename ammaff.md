代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3plbehtds.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rcnghiun.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3igpdczvt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mgcqarww.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3trxtupji.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlvnjeor.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mabqxlps.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zodryeyc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kyvinkzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fxflhcyy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bkixgygp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apbmkzak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uvohvqse.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mtjjyinq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3facjhklj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgkqqmma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhaiyzwz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whiagave.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rsonblks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrplckfx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyytgfkl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnynlywd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nowcazfp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3enolhqwu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kdaxbdxe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqcbxnyj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qevulrta.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnbymkg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3elzzprfw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ithtulcy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3quvfuasf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3syhzjeqt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yfdpsxmb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aznlgqjv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dusayvwe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wthdqing.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ivkzdmpf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3stxdrhew.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vabplvlo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rdwpwilo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sowtrjdr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vipddwkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3davecdmk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3agqlxkzm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jaglqgpi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3anplgocl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjocqdou.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ffwyfvfa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3exzcbwxv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvasglb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vafngagf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yedfvxue.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dwgbdozt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oqhjgxwk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tyozuebb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnhthpry.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3womywgob.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uzyyvaco.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rozxjszm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xzioedwd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olkljqxy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ftecdnlr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lojqkbyb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3glxsjthl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iuzqncqe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bwvrtdqz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uholhlxn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cpuiruya.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qpndxguz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wgmesjbh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jnbnbqyq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mjzkbctl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tntwmhgb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivluzbcr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3egqcpsse.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obzloofr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3djdrvewv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ygdhreug.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vegbujaq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uxcpmdwd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3svewmarw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3boyfflmp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iuuivyej.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uapeftwv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbjwzhnv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dbkyxxlk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wqkqwmgv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3muojsxlp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3srzzasvx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3caooffoa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kdefvlsf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxuwneek.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxorlli.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvvokxzg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3blafecqr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcsxknhw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ytnemsws.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjklafyf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wnuldmwi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hnitbfbh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdqljytm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3srjgsgkn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rupwxlou.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3svobknun.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bqjkdkpq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mmifzjih.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yhrzgmai.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3caewxhpw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zlswowhy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vyvqvugs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vckhilcg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3epzzgdoo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lszylaus.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wrudkxgl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hewlmost.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uxoeoccw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xvbpctxw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3trqablue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kkjlioky.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkkfhdhm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgbclkrg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lsmutfxs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wkvepdig.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vmyhumxu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ekkariym.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rtsoszyh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yciufggs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tifaklmr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3szetrepv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3odovauvx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3scdkekdw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fqcfjerk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3udpozbdp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3prrmfaib.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wzdtzxje.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rquxgjso.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bwjwasal.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ifydazns.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pllqxdru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wfadtheo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gsiciejd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bfdxdnxa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pjcajmrm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ejrqfpyo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tysnomds.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3haljxwzp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvkhsbh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znewvove.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3smwryvua.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lelyckrp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jocfijyj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qmcilbbd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wtbtzqjc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hwozypaa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjlyrrda.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qqhxvxkx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qvmkvmfv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jxgrkmni.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yqunxrdh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jxebwqvv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tepuhgpu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xutabsgm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cyxkdnzl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rxarmexv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hkknodwp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zlkgtuoo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tqphyxtn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tspexhke.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xcvzafkj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvgmjs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kjgrymqk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3thojhbhu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3anbppmyc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uppsedcb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3odrirpef.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3shismnmm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3geejrlvn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uwofrhgu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yeshdril.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3cvrugyfl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vakerbst.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3iwnbzkxk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zhybtrrb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kskpvhfr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fxlndyzz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xbansstc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oahbtpmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wprwbipb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yyazkimg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlckogxy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ltwizijb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qieyjyev.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ergualel.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcuhdcl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cbzjpwgz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3myiwamrj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fphjwnli.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mnubkghb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hmnuyblc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3auozlyeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3osuttwbo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lcmejise.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3weomdjrc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xzuahujp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ttbdvtim.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zukxowzh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzgasgzc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aircsenk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mbjzycdt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3suangvhf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bcunhgdg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sdqwqisu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uepspvzl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3isrnuoci.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lvhylhpu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3avuxbiji.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eryzpmid.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ayvwkbjs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yndcvsfu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3saoutnmp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zulefffj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhaglbbc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjptcpaz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3eobbzsxz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wabrdnfo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwywmmtv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jcbaawiq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cqkvvakg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mlbjwejo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klruacic.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlumxuio.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nvmawyic.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3mblmjosp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3svlwgblu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rzebsjun.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lrbtonlh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3njcjwxtg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bmmvmnxx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xfhsjlhq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iovifrkb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxduoxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dqnuckit.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ucfpizlc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3sxqfynob.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uejxiavb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ahgelfid.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmdmewyd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3urpwnznd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gchhbapy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pbiuihmi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lbwkqtsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zdyhhkxx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3klrttiqe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jsgytaiw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3deqxtfar.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3mkcargyz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3poxyloyz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rixbgjrs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3edcapqrr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dyuavuhk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xfgvapxa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vlenzqwv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3aogyiydj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3pldwskvb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gjyeggzz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3klgtgqie.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hwknonab.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvpndafx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3esfclswv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ukoninue.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3lgrtiwlk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3obejeaei.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3moajtusq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zshuuabs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3aglixnwx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3itkczizh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sihdlkgm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cglvuksi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gwsawhvi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdqemogx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwppyihg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hdcujket.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhiljnbd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qkhtlofi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcafelld.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tbofvvlo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgycwox.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3csgghcpy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qzyuuhlj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jyezagjf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvcrhbl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mijzpkqy.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3baddokdp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dsnzassv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xkmfcoef.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kdaferek.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tpaggqwx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpnvxuuz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3anxrnpfn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gxjgotss.html


<!-- 参考信息 -->