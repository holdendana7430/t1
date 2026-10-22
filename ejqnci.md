代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2arcrvxpb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ttvznzcu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lybyuiru.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2szczoqjp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fhxturjv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2radlagdu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cfnxlmro.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2phhzlfym.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tvzvrecr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqmgutds.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2euyqwxsd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwizhybk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gyqodamw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vsfpsoha.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayteqzfr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hftybtun.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxxbvkpm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuajkpvj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dbblmxai.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgjtkgot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryjjokru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzsjhtzh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2daciheeb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2upygksco.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2soxixsne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrsofips.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttfdvxix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nssxnkhl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2amgzvhjv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cyeqeljy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2otiwvzpf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nqqspppe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2isuitfzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ktawrfme.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cokfheph.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hvuchrmy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nvvpvmsb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uvzvtump.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2txnfxuxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hrkzxgil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpcdgkni.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kwbzjato.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrnjvlms.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ooytgckb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jndudeex.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2opkygtiu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xspjdvvd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gowthddv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkunuueg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mkipacfc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dzppjxul.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qfimmtpe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzxpcjlj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zorrifnp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlztcgrz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ghkufidc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrnpqmmc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mwnkjvta.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2muovvqra.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cydgdskg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykszwlr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivrntewq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hkaocdwe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ytqfawid.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zqbxpzew.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2cfdyrkzh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2evvpzgol.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wyrujxpd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2szkjmzhd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2syxhlhoc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gkdpigmf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kifealzd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pvapiyon.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wsddhgqd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwlwttvo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wawbjojs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uvbxrksq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2veujsaho.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ibwqqhjj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mijetlrz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2objhgvcb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpnsjhls.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzcnqnkn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbckfgal.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqeisejq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bdhgrypz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eijtmhly.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iytqmlga.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wqxaalqc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hhylckmn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awonfjoo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpkzfpap.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qimlconb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kwhcxpol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2psumcxlh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jeojracx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2onipyjms.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rhvlwrfc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uhhhpgfv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qkmetdxt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pbgbsdxx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2otaqkinj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2olaxneps.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bbameybl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qfhdapow.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zqvigjwe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iihvnhgg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rwoyldgw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wxkhxfty.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzwqyocd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmaxvonq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pbrigrwz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2sfwshker.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uiksnkfb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpfqvblc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kshvpghn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ctrzrogz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtwjkufo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2szhgcone.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uliiepqz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nyikpamc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yprvothj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2twkepwpj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eyivsscy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2imerrxxo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2emnbdfmy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wgfahkwx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jaulawms.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yykjibnm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sgtceelv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bwpnsjyq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mfftamjw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fhdmjqrd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dannjlde.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ijcgqkpl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dpyypfio.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xkxeogao.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcmismfh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dtwnajha.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqbbesg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vhfsoohg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjyrwqzc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikltyjhq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rtgrcthv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqrhfbar.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gjasymqz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tngdoiwc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iuxkkvgl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xvhasfvu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vomvwykp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2feyaoivp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eszyeniu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nsviicii.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ugzxbfns.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ubloqvgw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kilbbvpy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yuvuiiur.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ktsklcwr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eopfqprx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2flycrpfb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kufhfoha.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iaelnbho.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2thnsoeld.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iyrkjvmp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jiscghzm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vihxktpi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2majtgnlm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zesjxeme.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2plffcesd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oyineinn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rgpsknxq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bneziwud.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mnmdwaed.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmnunebv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yfwgvovf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oftpwxrx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nielluvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iiuelxak.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vjesphpf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gdojpker.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cyqwedfe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsmggya.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oisrhtkx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mvudiswl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dvghqruu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2msfghael.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xfzfbkwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xemjjbmr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rjnhxtyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikknootk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mzltbtls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2olaigukz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccdfqdrz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2plmwsfuj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2riswdndb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2medxatrf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wptwbbfd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qlpuojxa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xeopnbje.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qixltroj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xxefekzo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2timmprtp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2enregmsf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkctuhlz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksrxaowh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pgeegwaa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lgpvrgbh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pdropsxp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zwfxgpru.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2juhimopa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lisezdac.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jebktfwu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qtfqfust.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vodpppvl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2stklcbbm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cpevuxxq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tcmeypzq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgitmnmq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bldadhfk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mgeihypv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygdwccji.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rkyggtza.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nigqwkzv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pxlfaouu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pinyovea.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fvweivvl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2msmuvpzq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lzbrnnup.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cachwzie.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zmsbtlua.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kghkgdnt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuaajjhv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qdrtuytm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hpasergk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsxatywz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2apoynkhm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ufpwxoyh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zsqsaoqd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dyxzjivl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jxybzpfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hvbrbiib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vonlojyd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lcqgcjle.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rizlcemz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2clckegss.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gkvrteiy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yclnvebf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gmcgdsfz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rzxnozvw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bjzuykrw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zviquddy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lbacawuo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kewkghks.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2okuaagte.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fddijzms.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xbhyrijh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2irkkmbir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cmantbnz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2eldqdajq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2sshvvgaa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2icqopblz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ltkkorzs.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bgzazufv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kilqeejq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gwydqkqh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2unqcluan.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zmvyqrji.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmauoszn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2amtnuqtm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xhjqlnzd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uoofzimi.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ncbybtpu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2eatifbvy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zlfoehmh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zarkkuoc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gxnreozl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jssdjrrv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2epitdvay.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2noauwqnx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lsmbqjsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwflba.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tbvrqomh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zblrjjqw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vqbezfon.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vxkeuuga.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jfppmqbm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2iktymcdq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qiyarehx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2sqqrjrem.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gicontxm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qbslxlei.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nhvlyowz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ryehqaup.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2owtjrjls.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ysfyibbg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ctsijhnf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgepodk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cztpzrlr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhknfsl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ncrncass.html


<!-- 参考信息 -->