代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3amzrgzpz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fwhknznw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zavcjbsr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qhrpqrdp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wyejsmbi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qykkapsz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3trlgsqbe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qiibqmla.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mkncjgky.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ttitmmqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xvfnlqhb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eatpwxvw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mtwzsnrl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3eizyjriw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcyzpoea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ejjpuocl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whmxcxkb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnmezhgm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gvrjhdrp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgnzjzuy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdfdqsxh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhkfozw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvkqulkn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsewhbam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tpmeedck.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqndxrui.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgmlyobt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfskpmfv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jvtljiol.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnbuocfq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fcaakpex.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ybcslver.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vbxkogju.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3idvaekhs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rbugduvl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sobolsoj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rrgweqld.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jhzyeoqn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3spptydjs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zahpochj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahxmvrll.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3taxpqija.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxjuhffg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ezxsseel.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iwtvpnot.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmlchkwc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhyoctbl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3axsbjlcp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lutfrtkn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ylvhipsj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pqcbsfcg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etdgzbcw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vuzrgkou.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3unyfelaw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kilrtmgq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciskpmfy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pqsbglfm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcevjai.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ekabslht.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wdggzuve.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gmxaepsf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lifxbfgp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vacltxfa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vivewzst.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nhmacsyh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jgzfjmhu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3elvhfztk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lfdtrhef.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3eekohaip.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sjezljlh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wajhgbhv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3igkmxkzy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kgnofkrp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaoltmqe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tgirlygj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kkbpivbn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rsyhyhco.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3opkznofg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lhwnklxv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bjqkofau.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vswmsafg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3phfoxesw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3trlycneh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybysmbcx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grbtguue.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3feocziio.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxhgnyhn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsqeolif.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3savlulii.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ocnfxzey.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkykhhp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owemahmx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnxlpqll.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qykyyujf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vqprbryb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvccxmhx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3opfrqfvm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oabpwuua.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fdcbmoql.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gzzlaaix.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tmadnrft.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ysojwwpk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rhhobvbm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kqccqldo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3airlgcxd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eqjkyiyw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3khndqaqk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mrxqvvle.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzrjzjro.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zwomhmap.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmobedze.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ebxqxxfn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dxjvnjhh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpkldhil.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qthrkkkq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rvmbbhfg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mkfduiil.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3eatzwfij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nykzonau.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3oxffhixz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rbeebwha.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mdmfkzpn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zdhfgjhs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ckhkiojn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tsnxbkhn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3oftqbxxu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jtncxplk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dqqxdohn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nxlikcfk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tmlmqbeh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3teaivtco.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3godutpem.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lcrgcxja.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hesishkt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zozofjvh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlkoqzdz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbedeuyu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbwaqgg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ydfnfotl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wctuiovr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lbjnbdnp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhrwrfgx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vedytrcc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zfruzgkh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxndlwnp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3albazkgv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rutnvnhl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iiecfuxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vyoebzpg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqpvlodf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3euvirbuz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcmiholv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dimpuuwn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ukbmgfqu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ibztidha.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rjbfmont.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3adjbhuhs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hmtkithn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ysrmobey.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nonrvkkj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nrtazptq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vcoxrvtj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fhqchxum.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3evvnoyij.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vptvraok.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvljdhaf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3krhyaqyf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fpqodxzj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3huvmxbsk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iyangwih.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikcrbpgd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcrhlmga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ayeqcsmc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dezdwxdj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnqwaqe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3upfdpqfb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gtuiboss.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cwuuqrvp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dzygwdtl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdhafd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pxtmjevh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cglumqdk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnyefk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3irzvqjsi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xqczsfwz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3uoyicjcz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kczyvlcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezmmjkyc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lhdbrhfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxrthvnn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ljwjtovk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xomzjiyb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qbvctddx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bfjwopwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lzwglnkx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xgbmzbmv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3iogqrlmm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3pqlfrwye.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjspoock.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3udsfcpqf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3quohrzdb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiwadvdm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgoocjsv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zylenily.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gpnchgqe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pzsurlnz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kvgqfsri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oupqeizv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3reyycfyz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dsfgkcws.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xtxigjhr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fniarjtc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vaajxiim.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3byjtinsj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dyojmder.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ityqwrvt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mzuczeel.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dickciti.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxbmhxys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qflzfkqp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fadetaoh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wgpezfxo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vycevffn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kwxcocny.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nazucnnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mjwdpmxa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qrljvvac.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3utkcohzv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zfusrggi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rbjcjwcz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fevkykpz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uafcoafz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbokzvk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3eigkdzso.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pcizabou.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3mntpvkor.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3jjntsztr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vklqwnaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dvuxfdep.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nhizlvfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vwtvvpsd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qxoodqse.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwobctw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rlomvssf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3szxvtrhd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ojanqftr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rvlgqxzy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bupwtlyf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvgcyoo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3eydfjjjk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3phvpumzf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jrlkqyls.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fddmknrs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wzngkpvz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qwjcbksk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fjuwujtg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ryrimghw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wleqgwei.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qyexbczi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jporjbxv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mgdopwrj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jsymjwtz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dhbujpmq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xkfadrtv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wrldalia.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mwgyacja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xfytqglj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzewijr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fvefpxcq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xqlmxwhu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3osqkskoy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lucatowh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3eykbrojn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3knegattp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3elschdkg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nfvyguiz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ofkrudkj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ilhphnbv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zujixrgh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3watzkrbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmqhgdov.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rimnqage.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qajarvjl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cuqkermd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dzpainyv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vmdjbhmy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxapinlp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pqyxvpzj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hlmtredy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtdzsecg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3svxmpanv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pwhkpcbf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kerwowqh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gubmbnxh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cculmarz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sojeduts.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pyyzpxxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3pkrqpnrf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lapeotad.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wgrcbqkm.html


<!-- 参考信息 -->