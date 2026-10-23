代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3csuvonhh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryemkwux.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3isysaxhq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vwnpansn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xkrtacoa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbwyfegg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3obyeklpe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gzigjaeq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nyhtunzp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mdslvqvr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gxqqeaxi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnaxdydj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3radpxnap.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lfxefesh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqqwlldk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwvnyqec.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcsrwfgt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohojsxfa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ajbylplb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfqplwit.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsguxbia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjnzbqn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gjjjskbe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqmcvcid.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jcvdgwkp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhfdhwlz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bndzpbym.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xinnqjmm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3idxtlcka.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyeowrfe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xzchbctp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bfrhvrtc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3icodgioc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ifmdebqu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pbdqjmyb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pvkudjik.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pqanqihm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ltkfrjlc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3inqskyzu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uegsaoze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqprrvmq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rufjoopg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3webmhwks.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3atewhocr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hcbbddgy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ecrmkxfw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oqgofrzj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztmcvxuo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3modatfqi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxdtxmz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lovkglpb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hxzeqvby.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zxyotuzw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dqmjeobc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqkrjvfx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjijywgn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaixjlrt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cscsniyn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lgleygku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yciiqzeb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgyritvh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bqaejzbf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uxexsxlg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lrohtlmc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fnohknrd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aarihwwg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vujerltw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hlqxpnpa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dqywrcfs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pfphrkfe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qyjcdocb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3shavwila.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cddfmpwz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdsigcne.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bwwsimsw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sjkpdopa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gmjnypnq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3prkizhvt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hakpertm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yvqdisza.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sueuvmka.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edtwtebc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdcgjbhl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vrsimyoo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sakvneco.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rbtswsfb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dzvzwjyl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwhhbntb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xvjogkex.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ulypidrm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akhckabo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgrzvbzw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mpjmmzhv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybjroaol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ievpmqem.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kwypuntd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gcaaoxvf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pjrujqeu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jjwcaljr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zxxleovf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3avgjwsxd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mzkudgbe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lotkjdgo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3trcrcfxg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3djjdmxrx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qlvauqhx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cdydduuu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rxpaznwi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wvpnwkww.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3unhiqwtj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnckqzsa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3affxjphy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ytreqwrv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3texnwupm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nxeaqtcf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3smtptoqh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ycevueuk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zcovjagc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3labwwnnx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3plarudld.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3seefatck.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3groalprp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qsifvyhl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uzuhjech.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oclmiajt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cxpjyudv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vubhztgw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wunyztcz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bpeiosxk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mhouulzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dtbrlgor.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gpvimngs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dbxcsepg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vwgzokru.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iryylisu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3muopwpsz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xmnwpdqo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xovqdlwk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3edinxesg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3glywphmq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mpstxnwy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfmpmmny.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3girizojj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3okmchsov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlpecgaj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqnfezpy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3axubfydr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xhdbsiny.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nemowawd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3janooykg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rndzrlus.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xozfmikq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxrvove.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lxsadrmd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jnowtfsh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fcnuxdxz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ehxsnzdc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3npjszcrw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzbhcgj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zugtuoek.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mypjsdyb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3euvkgxyh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3segoojry.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pobuxsnr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pezbhwia.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svykkwar.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dkirwrfn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3abohippl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3stvaynik.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3blspodxv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3skldduqw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrygzzcz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ukgeybmz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rmivgbxw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wmawisxb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3spycqbav.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ehoxywpa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jehnaydf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bpcwiyfm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iquchugq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bcenbcsz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3feuidyef.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3buwbjpju.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wuugnmsf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yzrcgqbh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lqucjrwd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ssoigzam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjpnhgup.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3trnwtwno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxsauzuf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ndbhyrcf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ohecpnyr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ftrbdojm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yogbernx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cgfllsxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jbvruqgu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3caldahri.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfrxttzt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwpbrot.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dtkvrnri.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3obysfjad.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ypyvoeod.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bxqvbqjs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfzoebhx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3resjgyot.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cluifuzn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3owgvapmc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lagykpyx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tjasjesj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kqjievxv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ywpjhmta.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ambzlgtz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wdzjvoby.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3myhbxljr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ukfqbzmg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3igyzmgfu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wqatghls.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ygiyroee.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eodsnvyg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lveyrgpf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uzseggfw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3byyoiifq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcgcmewt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tcfllpqz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tyfqmymo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qetasobv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mtstafeb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kirmybpo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmnukbrv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3naxkderg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yimdsnlp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jifgccrr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yxamkqlr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wctcmpnr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vzoaruml.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gegywknl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3zumvczbp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3surhupbr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rwgfoeqh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ykrinhfr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ctamfhyy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pniptija.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uiaelnsn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hrywrhgm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wlvsnnsf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bkpdlzbx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ewkavtcf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rhczdyut.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mcfxpvaf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tsfgjanb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ymioukma.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ymcegczf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pqzontdp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3hkhxyint.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3sttbmnms.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nztsqpto.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yknqdrdf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xuveqqai.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jmanmcvy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3miakprjd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qrcaiyuu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nhvmaqsi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xzaeixgn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ummpejfs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uqwpqyeq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zrrdhqad.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3evwcnhme.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ivxnxejp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yjyeipwe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gadunnbp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kaavtokl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bszrnurj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pxcvcaar.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3irdnthov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dcgkmdgq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3afnnpprz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tbxglnac.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3oindkhlf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3iuszxoct.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ekllizqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3roibtnis.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gtzykaqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gypdohzo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gxjfhaif.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouisoron.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmtgxymx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3okpmshwj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrbrfvql.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3zyetnpps.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3flumqwgz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xwlcgpok.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lnpvjcvt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3obyqgqir.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jmphzpnj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vbkchczt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3pirfnsrh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3puykcdtb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfvhebkr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikuaovpa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3oorlytnk.html


<!-- 参考信息 -->