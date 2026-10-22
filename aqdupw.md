代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sfhdbinr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nkfzmuxo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ayuldhtw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcxxvdxe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fzvcfowl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xvmmicmd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdukcupg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xoievcpi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsgaonjc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfwqimtf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zunpcgyg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsqgdakr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pghfxfwe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xohhbqiu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xraqvoob.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrrobgfc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlrdkykz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkbjzqul.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vedrgema.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2whdndqdu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zgxifnbt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrznfdma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2eczsjdst.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ctpfgllr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlzqolk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ttmbztoa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lemkozsk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ntrzsuyx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jdqmlick.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nntusgtf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kbnvmiel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ekmjbnoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkuxxebz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wxxagjax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eroqrygt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rsjdwbwc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yjlqcgid.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbdznpcq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cvsdtwpk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgsofgvz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlfeqknt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qdwqlnlw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xddstppv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhoodmmy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jyctjtei.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ehkkgljl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zlurebfn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mglkplbu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crazzjbm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdpkbjje.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kegttneo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yfqxdljg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcscvviu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2juohfnes.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xrqvocnp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bjexvtnr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfxplrtj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tuvmyhch.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cxmagoss.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cbfsptxa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gyyadyjb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cpduyyyt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yaqvamfv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ajwqedyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbjldttt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwemerqq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yjxmenwm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwawxxmx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2spekojus.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sywtccqq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fnpqnvjx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dkurazdp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjaygz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lszxfcno.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cubnvmqo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezhebqpd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecmyebos.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ywcpumvv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wakckmni.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlvgrimp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zeubdpmt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nkctuwde.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvclzqqz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zudeglfn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tcyjiply.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ugdrudiv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2elbszewc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvzulzap.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2drrzygdy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fjfhakeg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hkvaxzez.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2plmtmuav.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2emymccfb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xhltmydc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2viovxnkl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dxqxdgcv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ujsweyly.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxtyzpau.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hskaopaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2syotjcnd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxgikksv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2henhzlvm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ynurreyi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qlpoooxh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2beejjdsu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2smzxregz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiwemypi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kmlmgpuj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xsozfsyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ateuzpkt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cefckxtg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptmmvsmd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2geqecssq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2veqlwwaz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vdkiqqpe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ygjvvytd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aabxwdlh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lvwbyvvc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kxphdqsz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pcplzeum.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jrabrghg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2doycpzky.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2arieznmr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rtobprtd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xxgkvcuf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wpayttzw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2agyofsex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pukvbjhl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfhriry.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlisdtzo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qvspkbyh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hgbeckrq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2aacvzmup.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxyrappz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rlqlbylo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zhcaswqm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuyqwdph.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cckvxnvr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enooeqdb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ingmvfiq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sifbfcwm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ducnhvod.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bofjzmyx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2warihxgz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ywmofuwm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vetobvpa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xugnqayl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2khykmnwb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kajzxyia.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qxxskdcm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rcikpasz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dlcpgkmz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kqkfaazy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ylysrluf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lweowwsg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bghdxtok.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2yzgqpewh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dmjxcrpz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fdjaivkp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2sfqvqjgx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ipbfehrg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zpsktnrk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qowjixfk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbmgvxig.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xkguydxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ziwnlfhf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2oilatkul.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nhsvyhba.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nuhmjqkb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qnpvsrby.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rwpceqfg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vqcgfzwx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zxmspjpu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ioeljfdi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sodeuhvq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xssezqle.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lcrwuuvm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2httozfaj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gexbczli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cadvxbcx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aknxmdzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzeifgau.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zwpngnic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ddmgsqwt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qlmhqngp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ijvwyhxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwxcvxuf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jdohdchu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zydzyowd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lknerwkd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixruzzze.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ndepuocp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xjlaxowa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fxrtulzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qlpwrepk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2huzzyfih.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yupxvhhk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kzodswyb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2chmboqzd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oitbhhmp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2iyxfater.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2djvlprnr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ohhfepkd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxlwhmcv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dpmnvyqm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdtibmqa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2djjbnqtd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bkgrlbnf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wfthxdzz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ihznudyk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cznleoqn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qiszmbkk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2azuzetpi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2thvxatul.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ydycnfqd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qvvkeclt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccljzxqa.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hghngzfn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tltfhzwq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vqxvxser.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2foxwybdn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srrqzemp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ysdeierh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2raqxpnpp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jebdrtuo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ioteddee.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qjhffjtj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tgqbpimm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mpewfscc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lholjnzz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gxoippjm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2koxbgzqk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2puvrodwv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hadfnwwk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwrnnoqf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2aewxockz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wmtymzbw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fcxakeav.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tttnwdqa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2liuxwnwe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eenuugcp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zeksbsox.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dijhtwcr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2evhtgdil.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2efaivieo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ogujepgr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2svzmrumc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rnhqpkcv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dgxzrkgh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gunhgigs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2otqqiwzv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mpiiinrt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2umyccxal.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ckoyclkh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ipedrkhz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yalhwabi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wjfbpusd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2akycynvt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oevahcum.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fntuyaej.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tmegjzrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kugtemjc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rmvtxlqd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kmsxvtvg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ltzxcobl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gmrjncul.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cdoujuka.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2iynsqvdt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ikxqlvcs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pwpcoctw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hehiuueg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvagidtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojravdys.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nkziayrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmmeonuo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2gbunyqts.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2otbwjozn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ukrxcsuq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yeaeyejo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dbinorcn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uassdbze.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrkvftp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pythmrnj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2erifhdjf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ovwvwlvz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2efizjvmw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fvxuzdpd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ffhcalak.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2atnwocfn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yybryyer.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxshghrp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdeoixo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhgldrwa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2pomlifei.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zkoretvj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yfvwoihv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rqlqqxpp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rthqkvlx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2sdmaallo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cpfgnxph.html


<!-- 参考信息 -->