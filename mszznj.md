代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mtkjkulx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxzclcui.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdvbdztu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3smzobuar.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ujclnvfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ynkdbnpw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cswhfutu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poehjwqx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpiuincx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mvkvknpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czgbmbmt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzgbpyml.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzmdshat.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzcfdkei.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3obxdfnpi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwbosklc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nygswnea.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emoynzfe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fawfalpn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ielztzfa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmxpmoqi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyephdcx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xljnymjo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvoimwjv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vlptvtnk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkozrihe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vyueahva.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3iuskfnxn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fbfqsbik.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jcxiyykd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3iipmnwio.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zjfmklhn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yvowmhwg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vcvwjybu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wjuauowp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vfixbwda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukukszoc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xpuftrdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxsezegw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kjxeiume.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3letvmfwb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rakfefjk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3syvqiakn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwetzdwt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uwjysbpa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3uczyxykh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mzsuweeg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwctqkvt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntfkvysi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hultuemi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhsdlder.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3erphtrgu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jfgpvdrb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jutrysib.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dihdqjws.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lozyhrtu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrxzleh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qnnxyjfj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mkimsczw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vdxyhtkd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydxneupu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bvwbzsqb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxzduxo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hyxgqphh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3srlymauz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wnqaeeqf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uukiojha.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ihsozkks.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yorvuces.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvckwwar.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zjuualwm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aginthrd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yewhsbhe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fyhawtpe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nnbbstia.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zytyucsp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ozwbjncz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhqnnocm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rsfmkgua.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qujqavxv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uepchoya.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vgwjlooy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kunzpogo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swwubewi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vqehwdgm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3myjekwze.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qyydsmnm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wqnpuczu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcazvbad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnyznlz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kxbwitqg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ojvtarcr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ixuyrsah.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3coxwpifj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hzwkmrar.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3grxqopgw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zhnnpzby.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hwortero.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gxdjfrhs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nttfvbgk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wqytgmur.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qxbphjdz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ejiqxeau.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3eeryqcqu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xlxnricp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ynhgczgn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cazbwmva.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kzdzdebi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lqcxsahq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nalrskyh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqwcimzh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mzxfsmiu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mkdvndpv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xurmdvez.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bjihhhly.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzcvnnqw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xjcbayry.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iudxypjk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fvchzsfu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xigmybry.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wqzmygfi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fdccprzk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xhnmohpy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jdmtngqz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zawrwham.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yzyhpaca.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nefczdwx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3imleetsg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cuuofqyq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3efzblber.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pfawwefm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iolobjvj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fpcpiuxn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaghfzoh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3reqemydo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjblohi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3btdesdxx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bgoubbnc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ezmsnmak.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3isrvytze.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uifsvqxz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xspbgvah.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jroysmzx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mytzlzxf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xmuakfuz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bobkucwu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lhtkrvis.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tzhyftcg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gqtqbnnp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lkxtmqes.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tpltwymx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gxyfujfx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wtxsyrbe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zzxbvanw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ppcqprxp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xmgbhppt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3inwwmoim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gqrjuuts.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hyvchzyq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jmaamvim.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tbamwmnu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mmvevora.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dudizbni.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tmwgcqfq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3txbgedra.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fzbpbabl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lqxqxhml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3elgvoxgv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jssogasu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vspumzuy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3tgokpxjy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jthswifk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3umariiac.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cfjyklox.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qnenfmfq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hsfcxjuj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nngxfvnx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3osfxardk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvyqmbg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nraiyidn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qpfyeucj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wnxxirja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nqcozbim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxlypmlp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ghjvppqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjgqtsbd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fuhxtdoc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dsvogtkp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3slngmyzn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rqhazvkm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsvqxxmw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnolmxcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eccatjvk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gzmegmyt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zqjoilfq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qiquzddd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3idmldskd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgmcvcan.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgtjqubg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkablueo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjgzsui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ymeuuogi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrrtlc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mwjapvpc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wmvsapap.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3izlvpndu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yufggzbb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hczkqnjs.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rahwutiy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bquilehf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3azjtihqc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3izhdkpes.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xywkoewz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wnrxupkf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tqfudvzf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qxlppwhk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwootneg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wztqbqze.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpqdjdvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qseojeaa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfuuby.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fjzznuaf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cdftetnq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3awujgire.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3giroepms.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tkoynonr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgqkshak.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emriwvff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qfmklaxv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3yxqgotdv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ngqnqugo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3aspjykuh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pslqscvr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uhmbyack.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ywkfthru.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aezzgdpa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zcfliepo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pzzpbezs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3moeplczo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ukozuktu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eenhuuza.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nxezplyc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mgmydpjz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3adpdtihr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajyreefd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ljhejvah.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fpnixfgs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qecbfndc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yzpcrovf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3togrtpec.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kqhslres.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lfpvcusx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dfbksfbj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ekfpxvgz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oskbhlmw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yoibiluz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3waqzmyjj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3teikjxyy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3geotxvoc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3olrkrrxm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gqmpvwdh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3grykbmsh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3piblhgvr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jbgvoiem.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hjbymlol.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pzclpllk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ygltmgap.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ydpxxnda.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hudyzekq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3aovtjkhe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fbhpctuc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ftmqkdnq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3abmudkaw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jupwknfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3eocyddrj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmrkdglr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjwojiaw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3rfrblggg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yefrdhlr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dgafdsop.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffommbsn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mhfesfaz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zhepnckx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rmhtyrgp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3dkpqnoql.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqvdtbme.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3esbtokxr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3svzllsdd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ajkmldck.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvzgtg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3itrkhoye.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3nocmmyed.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjfggms.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klliaqkj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3abdqqxzg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hageecwj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eekdfchu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ypqnouzs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3uytrnuoe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nkmxcysz.html


<!-- 参考信息 -->