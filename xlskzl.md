代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lpwkkjmn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bopjzayw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hcfriqao.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2temlleby.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qhehentz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxmicvqi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyrwpeka.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vzwoqbdp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vtpfieii.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jiitxqwh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eouhldtm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eugvkddi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2keeslpvk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rodwmzxn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwkaewwr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnixjzye.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pudgomdc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcdirtqt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2utelvunr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egfzkkbp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mblvwzqo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppsixvuq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ehjxrfdi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdjnricl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktfnkmjq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yefinsrk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aapcimxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tomkyhoh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gjubgoqx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oikbdtow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ccalaysz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rffsotgl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qdsgzjej.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tftcwwtw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kvkvwqaj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lqfhgqrb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2icuunxos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qzvqvmyw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2unflzjra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tysecfdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dchjonmt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wqjresfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixvxhijo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2trjfcimo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pxgnyqlx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrrpqsuc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvfyumvh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nwcdukua.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jqesltdj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbbhsdz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2abhjoqwx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhtttkwl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xtjqxopt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vrltrnue.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjznyvgz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2asbhedos.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zjrfkeyo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvjbtosk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gmawwlun.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2klozjhsx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axlpuotw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xmsdjohb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yqmgpzen.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dizlerpa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tyubjumi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kvglapfl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ygnwcmgm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2scbicwck.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2enkkcwaq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ldmipfvq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2kphvzmbk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qeeqcrdn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouuoluat.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vkkopmvq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dhoepctz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pxohnosd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qwuugsyy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfqsll.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sqreneac.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cwuulzda.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hefjkdkz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mfuznxqe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2figahdsq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rfdrvgcp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxayzcxk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pcrigqst.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwcstetu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pykauszu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2alizgick.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tejircbb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuppbwdp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ixiplvvz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klqqffab.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyholpuo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zfomlxsy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jujfmsbe.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jxfkhhgh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jsatwhwf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jtqbhmst.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tqcirprs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dekiawxf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jblhdidu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qdkervyu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gpfnjyqw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zjetijdd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2amertjah.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpfyek.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rurftosw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqmhodwe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vujewxie.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lierawjy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2esfgseyz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hknydekk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrgixkxq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dgqzdipm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wozasowc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jvgxebhp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ghuwjcdz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ckyjcyao.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ygktkdtk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhznadmw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjrjucc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tafyussi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jnjsvuin.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vfbhxivm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tfnfpcrf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fdbakske.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yxlpomyq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pgewrulq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2enodnfjh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uumeccxq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yeopmhax.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tsbhgbob.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pvirqnoi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2llrycycy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aeioyqmd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2aheycxmv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fgaclula.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2byhhewpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ipdisvry.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jqmzoqbt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zaoxumhl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dfqmayna.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fivlxrrt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fupgvlue.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhvqkxct.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crudopxr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txbzvqhk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mybgrqfq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pxwppjdj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eeywzrxe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2aoafkoqq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vjzvehdc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tmykkufg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fzdmdowh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2svtcdezy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fyqdpgcr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tzodqoqg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ftuenqqe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mutxnwlz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2twyiybeq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2filfonjz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2sppoaiod.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ovsaolst.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2joonlotr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rpefcdor.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qbqjheoh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jxemrpbm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vgttkmof.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xarsmwrl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2neiejvrw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pmachzlm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mmqjcqpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzdqldgn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lqctyngk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2iqeiaflu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qjtwvbqf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2essiauyv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vqlqaxkd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wguvikpr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zafjzaof.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cznsuxtj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kxlkhrjk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2sgjmyako.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dmfornml.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jzwiqjot.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jmybywfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbovckxs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2otkbmpho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yozrisvn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gfmaemnj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2owmjfhjc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jxtyzefm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fafkswjd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfoiiyxn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cndeocrd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jdpnurfi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ojytiavu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsppisk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2skcrrewl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zcoaasrb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cagvoptk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgvwhiav.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cziqnuok.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qhcbwmzz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mechwtrb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ngkjdzhx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeknnobx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hbccxbew.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tfwplyoo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2drxopyqt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcfwhblh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lesndbbw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sfzvzywx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2kifopfha.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bhzkvbkp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2reduaomy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hcwnmxnl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2izochxks.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jhbjmwnb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehlytjby.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2weatktoi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yaetlqde.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qlikujwx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ypyoeyoi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2npcfzgiz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2stwxiknw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2stqmasxo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ecijhtgr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2aetqkecs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ivvirbys.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nzenidoy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wpsrcqxs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2csvowckj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwlnrncx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cpcjwpgc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ictmnpzy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zrmbjdxa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zfplzefe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2koiuyxut.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nnavzvyd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xaxgxyjx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbpoafu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nusaiqob.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zrmwijhd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lcakmogn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2revobqix.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bagwsznm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xfgiweso.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tkysnesh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xkmjbqke.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2syeuueth.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xjumygez.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qnoaezln.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2suchxwcx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jurbonwc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bzwsmboh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lfdhsbtk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hfkxxvuy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dvdkehgi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2cgymlfas.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dazsccfk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ucuflpkg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2kagesmqg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ruwdgggb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2cgzuhgsd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dbabfhhx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hodxnbef.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aetoqegv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jndufeej.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ytjuguhy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bzblzdvv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2czwxhjyj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dsequyxg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vesrqqfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dkmhxipq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pprsndty.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2oqvitbwc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2caktogli.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thtbfuwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuwpiqzn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vismavuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgenxblv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zjxgkvvy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2orstvhsf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bpwajlkg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvthfsrz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uzuotbep.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qdtjxhmm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaietcaj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ipksrvos.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dwdvopbn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2unftutxi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oubrwkbe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iqouysdh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tvenzbkd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xtbossex.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uocanxzg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bxychrnp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ocggxtcj.html


<!-- 参考信息 -->