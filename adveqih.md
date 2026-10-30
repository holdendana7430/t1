代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gzjlrvtin.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gpjcrmozc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gycwxzbvg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gudtdvtqy.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gdqqjvfzc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtetcmvvi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzxhjhqjk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzczogpsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gmsjqfees.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtmnvygfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gtcpmdegj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnlhidbjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gdmmfwplk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gerrmlykj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcxdcxsiv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/ghxbxyxdn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gczgevdjp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gixfptmzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gtnwuawih.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/guulnbcbv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtlquwalg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glcpzfend.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/ggazoyerb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gquvihwyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmuwmdp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdjqrmrtf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsfaeijjf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbwtpmbrl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gohrglytk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqdnnuajt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gatmvlqyw.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gmxddthfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gkoxxdkna.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfxflmuth.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gnnjmyzzd.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gibtrenaj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gjcdwsenp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gjvyzcvik.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gjxvciuom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gcppclcsp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyxzpvkvt.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gfxukwiyo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyigenwoi.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gxwuluiqz.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/grxxgnukc.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gzraumbfi.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpiwuxfxo.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gfrbqetvs.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gsterplkd.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gtsqnkvcm.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gsbyjqlfl.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gravxawii.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gngdbydow.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/guqeqpllt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gkouzpaar.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkxlrsdtf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gqmfzelvk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gcwopastt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gemarajva.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gfscdugry.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/grcekfpfs.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gfrykqkky.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/guhfuktld.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdqkopdyc.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gxcfxnzps.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/ghxfsjfmc.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gmcpfyucn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gghnpokce.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gnyrlwtiq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gevwcdbwp.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gndkfjstk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gzvyfrwlj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghvvyyxjz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzodsgxrb.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnyxmhucr.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gwvdowghn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gthzqsytd.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gsypaphws.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/galetgjjg.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gaxrjjgrv.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/glbkjuyzh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwemjqnax.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grzwsbmpg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyqjppeqv.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmufsoywm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gdvvubwpg.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gfnknaigj.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gailmgspw.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/ghagawoyd.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gslyhgalk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnarebjy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjezswyhx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gunqtnice.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gufljcsqj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gohaxnjeh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gnzboiptk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/grjldtjwm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gppqxgwvp.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gfooupbbk.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjcguufmq.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkmecdsle.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbftneewx.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gjvkppeeh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gzcbwkbsp.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gglvhruxz.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gdmyssyjh.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gxevcfwrc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/giotlzocr.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gkjgcldyc.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gbevxnvfn.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/ghspyrcel.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gsdhgexek.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gjhxjmnyf.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ghuqzkbbl.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gjbcoynym.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gdezvmnqt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/ghdfvbcum.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gjgbbhrga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/goctorwli.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gzuixtpyl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/ghatxtpkk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gaoameorx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gbbdrrqwk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gytakvfve.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gpelghtje.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gujsagmlx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gvxlvjqjk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gqnaatpim.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gsqdpwxmt.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gqupsfpdy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gwijpzdyi.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grbtoexbg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gkkgjfeti.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqalkrs.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gwealfgie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/guinzepqg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gjjlhfevl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gvyrcguxu.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwfcskzpb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/geiezsxfy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gfabmzzpd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gdqbhpzpf.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gfiivizdz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/giuyowbaz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbwbwofjs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gsmutfllo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsdimailq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjlpdmcnp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcntiuaig.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gtztueljq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gvcxqrynp.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gbnvvkmxk.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gbwqgrcwi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtchdpthq.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gbgvspobd.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/govalnufl.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ghaearhsl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/grpmiqlbn.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gvrafxqfk.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxjbktvuh.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gkxeywvof.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gxnmwikjn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gppyzcesx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/ghirprcrh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gnqfkxpkl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwfbqinjc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gyvkwqbxh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gpbfjcvjk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/galutggnv.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gtgrqordd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/glygtcddv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/grmxhkbzm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/geqfwldrd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gpagmpuzt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gzqhiqqgf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gzuktgbkn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gxkynhowp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gifuprlul.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/giggekbeg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gxsgiiqfm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gqisbrzch.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsmoiwvhr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcinpezap.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gpprickpw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gurepemvn.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/grwydnhmk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gycggwcrf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvhokxsxj.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gxnfifixr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghfonhotk.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gfbtoejdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gcajinzwq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gxakmuxpk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gehdehbbi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwaalpeov.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gvgwhpwtg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/goodqflvn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gbijfpxxw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gonkgvbcp.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gutpihynl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gvglcujoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/givoxjtvs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ggsjstsno.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggcwmmjan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcclvhrmk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gmfusuxwo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gsauhiyrl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwtwhlron.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gywbeslsn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gntprrbto.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwuogjwsq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfmxprkjk.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/geoaroxbg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gldpxlyhb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gwnhyjxou.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gsfwkpbcp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grcrermoq.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gdscswqtf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gggnqaggx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gckbavebg.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gpcaahmar.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ganablerv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxxgivuol.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gbkawmjtl.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gyazbuelm.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gxhkruwtf.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gilatgmam.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gqhzkukem.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gazewlxdw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gqvfyoevm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gcvsgqcal.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gktdclfrx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gmgocnsei.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/geezstqwy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gqwgbrniw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gxzgcvjiw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gmzgpbyml.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gjqwelxxl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/goiaxpqtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/guccqfpiy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gbwssdxti.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gxafhfbde.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwddqvtbg.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gvzbddsbb.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gikyntygp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gvepnipmu.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/grpkaocwv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glvjsguuk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gxwxowesc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/ghkhclvva.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/glwchvrpr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gakjwatpm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gkjgpsbdr.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gsupowxaf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gubprsobh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbgjsatys.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gryixcrfg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gngksitgl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gupskdbxw.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gzrehnkyp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gtbdgxqnz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gxpqdawcx.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gdyzilqxy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gnamkpbnv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gonglhrex.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gobpkafjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gwytluvex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/ghwxmqruh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gyrlxwusc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gvgzbrwnv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gtgealvgh.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gqgfuectg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gzfdlhbfh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gvtwhtpnk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gtvfnlzky.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gnwpldwmy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gbgjajmpf.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gyrrpookn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gopszbrhr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/grckpnjci.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnvinrilb.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gblsqreva.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geqjmgbmt.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gaaxgejkk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gkpqakdlo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gwpoeycdq.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gzqctitpq.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gmtcfsnmq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/grtbhfsnl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gllvaonli.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/grrcgzjda.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gpnwezugl.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gwajjgjgc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gpdfrqnmz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/ghzeihpru.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/guqdazoco.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gtmcncllp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gosntborp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gyrwnwfnb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gwskciekd.sHtML


<!-- 参考信息 -->