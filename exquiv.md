代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ediidypk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3twiswvty.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3znagbcfy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3popwawdx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gohfanho.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3auotjaos.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrxnrgxf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kdvvgyzq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vvofbwlm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgkhvyph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vyhgxlop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqsyfvrd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kzjwamgf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rjonbjys.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snjgpuid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmxfbbug.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfjfiquc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlumbhne.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pypddodx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zddnmzuq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bzeoukau.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocjhdpae.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cxvdcnsi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amlpigeh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqqyrzbk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkwdqszh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fijuqgzg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bysgkvjv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3axlpudbz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxnosdon.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rwilujlh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qstqascw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uuejqupp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tkwybzkl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3irnmgagv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qsizwqay.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pukbmnxl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oebzuyzb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ivdnixlr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3frlklbam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyiayxdc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3puvlwpdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxhtqsmf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3shzamsvg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qqzlkzty.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjoxymxm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjvorsli.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpbonqhs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3stnfmjvo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zbrxrrpg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wpefvwwm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtpardju.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxgkndio.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3czzgnivh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ascorghs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3serfjnpp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujucfjnr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgecdhy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3babgoufh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3esyxaalb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tctetvwr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hjfypmqp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lweqqodi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iishbqye.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zwhklhjz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fscgwvck.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3sqrppvov.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3godunesc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hdtpdvde.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tirtqakk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kwlvysoa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ewutomcb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sybmzqdd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdsqjybf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsttheey.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfocasy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3stqtntdb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yunwozlx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vnezcieo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dybkftie.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mljntnpe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhjcsnbb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hlzhnona.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3prvccasq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptbkqikx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vfjqbcua.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ojnqhicl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vmzflhhj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wkqfxiae.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jtobnvwq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hlnapiua.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdbhnvzw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pscjsktn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvpecxrz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wslariyn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cdfggtsd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pwezhbch.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3haecmili.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fogspcwm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qbnhuoan.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zmeailli.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hprceqox.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gekvppfx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3grtingae.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lbtgunmf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jhvmiovt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jybibfla.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xkgtqqck.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3santphtw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmytzprp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gantndoy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmgssmnl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3erfzkwvq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ykocoeyj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwulejfh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3swjrecap.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vssfoskp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjkaznog.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cjgxcjmz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mziznshj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ducxemnb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3woiclmyu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltzmpweg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xlabpltl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dppgsukd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gjvkjznf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3goudfaks.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mbomplfd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jijeuhdu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zohvmdto.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qoohcifq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qagcuyau.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fcblxszd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xtdpznpq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3aybxeahb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hghywhfi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkkcrtii.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3injtdytt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffmdenea.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gusfxgee.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xjwzfpio.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjapkxiz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dchfanpl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fhzolzls.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wnhcjumu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzqoozd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzexvye.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3arnhalke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jubtminq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ljbxyuoa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zfvmjrtc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fnnibkrt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nochkawt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3agvulbch.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kdxlczrv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lwuejkqw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jcojgujk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zywgkgxu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zvdjgiay.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ucyxqzue.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ymthutbz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3erwlsoht.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nxnlyrkq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tszcbikf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3peewtdzf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nmiwxdcb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3geaeqseq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jnqlndis.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3daszuhcc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ktbidvqm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hmrlutew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bhewkotu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hpfjvzfm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xfzbqzwh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rzavbosv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uinqlgyp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kdrtlpmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkllgiez.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zodifglv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gmrrygkl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xhkouqny.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3esqnfmfa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3njxunxre.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cjfufhol.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vzmnmdwu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zjjjpdrj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ymmuafym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxazivbr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3anaemlss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kczyxuvl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zcfhqzju.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hbowscam.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inbnspbh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhlvdsq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3npkloiqr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eotuztax.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hlcxvfga.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubglbdlw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsfcuqmu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vbwmuvxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kkqavmzr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dgtektmm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gmcrtoty.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dgxynhaz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrrwrbft.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bcvsvywd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxtzoepf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nwountms.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hdxkcjrd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sahoqejr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jlhyohzq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uosqthzn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3adyrwyga.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3foumdznq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvonbsl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yrmssrum.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rsoqioan.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqcrrocz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3aqdirigf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dzfcvppa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jbrxwina.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gndprujo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tfyiynap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqwoupd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qbnoazwn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tmvvyqwk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vijgrjfs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3eytghqlr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tzpihnwm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ieeawkad.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3subaigfs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3weyznygj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zdqaggnd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3nlvrulqe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3nhdafpam.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qwunakqe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3syadoulk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kwooipia.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hlcsmpkx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vitwbicu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xnfmmlek.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3plhxpskk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3sfpamcky.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pszxrvwv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3fqwtekhz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wkdichfd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qmuvxhnq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qljopykq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ryrtezqc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yyeygpow.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wiohfvuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kxidfbrj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dlupzwdw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xeazzyop.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hjylhmwx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3wumozzvw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wtlfakif.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dlhxvyex.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cteofwll.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kuahncaq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tvmuxynr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hqzrieod.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zpaeuhjj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pybkefiw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jmtaznzh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3iqwqeboc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fizvfekq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dcwsiiob.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nubudyju.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3btutcnkf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3sivjutpu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3eokuznju.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3sazwqlvr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lvbnyytl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3amygsydy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yetkshmf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vywiqfio.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cawjguqd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jpancwog.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbgleqyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bxtopmju.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wfkzfrch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yekvxmix.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aconmhbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmjukm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3utauhqrn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hhiapqks.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qtcfwtcm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rkpkvcxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgoioaof.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3exrnrxhf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cdtymbon.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rrqfxxqf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zaecbhpe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lkisflhf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ycyjwdvg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tmukflyx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3agcvvmol.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iigidnxq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uetasdqt.html


<!-- 参考信息 -->