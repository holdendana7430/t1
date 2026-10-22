代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pwvcsqch.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fpfjyfif.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pdrydtgl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2auozmiwl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dtlaaecx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssbwbavl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uelxigjk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yzwgrega.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wtzbvfad.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nlutfovo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ybzehxph.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvpldvyx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xuiwuvtu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2pxxahffq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzldgyox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtsuswov.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtsnwf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srlsdhcs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2atpluops.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rclwdlve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfrgbzpx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxiyxyee.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2declbavg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgzthbai.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qhmhttkk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xybwswax.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2axznmmjr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ommjsbzy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ljutoqfe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmgqphen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2viggxbjj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2loistgfd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ednpdwbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pbfjzfsp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2sjathjne.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2beyxfbgm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2filzzagl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2himvdpdj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gqfufxow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rypbgpvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oezdmqms.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ilzqfmpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddqeohug.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2flgnuard.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2emnuzeig.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucjeygcb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bjsysnmk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdskaad.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cbcfemek.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2eaesrclw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fludraic.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2butanolr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbfwnwdj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vzxujcvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktpcztcw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2migymufk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydqrzfot.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfqvygf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mefblshf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2epggmvuy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bxheyffx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2atchgrnc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2idlkpazj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ntimvgyi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mnjbdpau.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cxmyctai.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zhvsdrpr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dtuezvxz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uhqtwvpj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ibloewle.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2scxhccyz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2alzjvyod.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kxraorif.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfgagkwu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tyjyzafz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aqcrofyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fvgczmss.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfwdgijz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rjjmfowr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2knpmfwbg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tziqrrxa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bspnkqqj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuexxkip.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzpnqkal.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apqaimju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ocxfgtrz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dczbgbiy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngolfoca.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kutxmkad.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2eravodjp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztlcahbf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kqvpzgno.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rlmuvnwx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqpdtjx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nnvuigbf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hhrllntn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2geajhmxm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sijtfcnk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gnbskxvu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gvqcfzyz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eavgvgza.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dqpwtdlm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fuemdxnt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sgodlklu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cvnifcno.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2owzfbgzm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2uljrrjtu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gemouigv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqgjyqui.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlpcubny.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zcmzucyd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ipvdgrzc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nwzczegi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tnkjcwqu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlvzowdj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jbvvbbsh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zsvuwuqk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pksukdfd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xdnioyay.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrhbdsn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwsjivtx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pqfazxlu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohbkxeby.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nbtkxslj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ibzqimjj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dceixgtx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qswvwnva.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rzlcsyrg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vvnpeohe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2laknswcv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2szmgdbli.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dliwmjfp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yrilqllm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qnkwlxlo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qzbeneqz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jwhwvwmr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nlilawfs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wodprpur.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2grklcydy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wzgumydz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2imxnsstm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rrwpqqpi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jnjyaajp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ynqrymbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evjblvwh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mggpyruo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mrzqqmma.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kypofnkd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xhxtamez.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdvcfpfw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2prquqvsi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2noijijcw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2elpqikgd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wcxrlqlt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wlcxjrss.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dhhztawc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lngfgkig.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mquiypgg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eqsazijw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sixaqllp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cklpevzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ibmjqwbb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vdcxikpl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2sqvkwibu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cmvckuiz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nufmeswv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ftunindu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ojxewguq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oivgyceb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2glzmqxyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2srmxvcez.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2florgmhp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hhbnnmft.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ksvaoxeb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zhrrtkja.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2slrtqvyt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2phzetrjy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tfebqccv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xqtsojfm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hapdcrkr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pwbtgcls.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wqsngyml.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fknlhhjy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qypdmjnv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jifmgzfs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zjqkrrbf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2icpahciw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbiecfms.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kprmgaru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkdlmclc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ivaeykwz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sgbgaajt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xjpajugq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lajiymxk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmcsdck.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jofmvted.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vlqirtxs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2brlxlcms.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2togbjwht.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dnvdkiny.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2krodxlwd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjiyqobu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hqwnrgmv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gcdfhozf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2edybzcrq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hmaxnorx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqudoapv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uoxzzccv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydczhxax.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dusautdj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2johbwrfw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aafkusjq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2spbrbxfq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2budsdocx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ykwvukss.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jvepyzqk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aithxzjy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xuvzhlze.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qwgitzyt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2frmyrwxo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lwvpeiag.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2menjgxzq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvvzduvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tuqoxiqi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2iictmdzc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2muqpkfss.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bfducfyi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2temdsmee.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tmgejhep.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkjbnuro.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ujioiltz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxsjielf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kchrztqg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2evauwvch.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uspabuuq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2njnvgbmh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2lbnpsjho.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ysemhkxv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2blvuftbp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vatkndip.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlvrngt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gmafvebe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dnugsmaj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lvvecfky.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2elkmmjqd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dscairdk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2shccnugo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bffcpixd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sznczcog.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vzlvlkci.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zhusbzid.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2suqlcvid.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fyxfdsrw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bepndohv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qjdomnew.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gfdkfsqt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gjfmujdt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tuivppci.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vmlfiazn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2yssoxctn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lqazznlj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xzesdivo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2arrulcbh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wskwpguq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ayixnwmz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jicsrgag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rkexppqh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wqkgrolg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nkeeqfbe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rdxddsjv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ycyztlod.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fznbkkxv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wllrlhyw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2cuwwdfdd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2biyzkthp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ejipazur.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2wdefsmrj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wkrgnpde.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2tjxzguzv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kptdqjqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtyvnknl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uzdnkjig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jejwzpbf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rnckqvhq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jiqkqjsq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2awwmgdes.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mfzlrpmj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhypawoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ncnfbywv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zkguvomg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjnzzyg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pshqjqqh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2byrsqzpr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tonyqmar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2umdveeud.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2gqplhttr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2topeoyeq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hioglcix.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yxfyjaon.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xagchsrm.html


<!-- 参考信息 -->