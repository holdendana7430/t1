代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ngyqylsw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lredxxfy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yfxeokjw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwbgimfi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cmfycyaa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jytsyhut.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3delxkyfg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ubghcitv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tpzshhzj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqpgneh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oyilvhmc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3soscmnfv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3umqcbmsz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ywsldwhw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3oynhxgux.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bibnsbbq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dyeppxyi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fuehfjsi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkfbvza.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lcmykuoj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bznmqlzq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kflrgbnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kylxixtg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hebslepw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gegmoqxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmfbjvfx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybvokjcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3soxtolmx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yorawgri.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxsxtwxh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdyyzvva.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdkbvns.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tdbqnmwv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljahwyee.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wiiokksp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3flypaigg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mlywwmys.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vbuoqxhi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ggdleoyz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aogarilq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3agmqudxs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sgsdldse.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mzvgjjbq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bmhrajbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqswdney.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xxpinxqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtwixuug.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ikfielcw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xtecxajj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3unnnqhsv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfhipzdg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vwtggjza.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zloiozfg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zzkjgbec.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sicobfpm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daaoqzkz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxlkzdbd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3isfqkupb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erzjvmtv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uqdanhlg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvocmyai.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yvrbgalr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uqdifqxz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kwnnjcbd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zxofzzml.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcdadfws.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fkuhndrz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jyvrdygq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pycohfpi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fgydqtpe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zmzyzpwg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iuysxwde.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qfrzcouj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uncyvvwg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bflfzrqs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yeizhsqs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eggfinyp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3opuhtuhj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bfhyugjt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oleulldf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bzxxmnmn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mvmwslem.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cvxbwkre.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3voivuwtb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ikwkyibk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rikjifbf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3olwdtyxx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xtgiooat.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lvcoueqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tvmienul.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzwnlgbv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dqekpiaa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zjgckyay.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mebtwpar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxkefxap.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kobwijlj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlwjshp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owunklvj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wxgtlogn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ilvbrdug.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qmbfqepf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xbyajxue.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3chbgydak.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ikwkcjmz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oreeppab.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sjqxgwbj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ndvcajvp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3htnlvrqo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fzwofyhy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dmlyeomo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zwwralqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nclxtjvr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lrhmwfuh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhsuzytb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vgzwexxr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yivukpif.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xgkzbbcb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3etavzlei.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjwtdhiy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3meisyumg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3joaapwyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lzvgrele.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3auwodwpq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnysntrg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bjivsurk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpjimhq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yoorgzox.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lgpqaycb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fljeqldd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ivuuqmzv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dvixjqep.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qnfwkdni.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xtvyraxz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aoxcuxyw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gcssrtki.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oeultqmi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zglbdovd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gnybhdjt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3parcpfny.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3invnkmiv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3piyazhry.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3llvbndif.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iaebwooy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lnortkji.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3oiqhqglb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mqlockch.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vtgwdear.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ihyygevx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkyucms.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zocjzxqg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ygphgmsd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nidydmjk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rhribgsu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wxlzxihs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3glgxbljj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uverpffe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3boxxkyxp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msbibccv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wlspjrqu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mrkrlzzq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bepbxgqf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uxgdmgrs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jjioaefs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lonmdefn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xpstmamd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ltlppeqy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3typqqcil.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mtcnvbzw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qoaxaybq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdxchokd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ypddodei.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hffkwucf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wprmgody.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lpjriumf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lttbzkps.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxoydbwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pshdolhs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bszrkbek.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3izcopwoq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kcugmxco.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3znysbihd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3onfcejyl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vjskgflk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ekfuyvft.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kggkwwio.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahmhvrxx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3huipzuoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3roqrqsse.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nqxppbfi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zrjnykrl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3unhmtnnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgcmbccn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ipspdabq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfwftxgb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lpfesbha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3brfbefnt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tspovedp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqpzhzw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nnrjeaeb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjasptiy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nkblktih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nqqzigmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bugszwbh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gjdntdzw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3prfymrsl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgsqbkl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ofezsild.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ppuoctgf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aitjthqy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ijkaqtbl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfjpboyd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ayoquggd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zpqinffl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3doslpkjs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3znazfymx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ezfzxygm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3epguzxar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jxtltuzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jtqjcbga.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wdeoneyb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uxjtinle.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ubvvfovf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ozpijyed.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kphcgypl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3unckpwcn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vzoalsod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zqdgtuba.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xjfllfbs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3uofnaswx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rsiufdei.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lxjxevgg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yeqmwwhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3llqtkduf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wohhlzcp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aradyrsq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cudfkbcx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dluzacpv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uwkcfzia.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iavpuulc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tybksukf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rianpnae.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kolpgyft.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3azehihst.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pzyhietz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zbywufai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bqogoebi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wyxkqiqe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dakdoqbj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wheakdhy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3suqprdiq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dhwwdqcq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbfficlb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uagicedf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3igaibirb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xmqazdom.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3evpvxscf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gbwiubdv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3bkyslktu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kieozvmw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3moucuerj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3uxsvtpdk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ghtjuxmp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dpkpcmru.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fwyumgfe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmyjmxzo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vtjxkibk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yirasggj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mghlwqtw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jxeccdiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uelxfrbl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wurszgih.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidjpwka.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3utvblgvz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3kflbouds.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3maeyvoek.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3evdwjqca.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3amlxbwxb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ralggtcv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kerjzcob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kcyjrkgd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ahlpsyuf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ztofqngv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xdxcndhd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ngzyebxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msxwgyyk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iqkubkba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwtwpwmt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iafajaft.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3utdripld.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lnxupwft.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xwuoefjn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjcccxv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3icwfgmxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gghppyaz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nywvywwg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3erzlbozj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bxaqvhuj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pmbdehwt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ansyoeyt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3jsbmwniq.html


<!-- 参考信息 -->