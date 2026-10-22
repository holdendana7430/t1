代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2agctflbb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hgdtruzt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bofjhccx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zivfisph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yonomkyy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yustriaw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2clprqazp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgyyygxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdmeaswz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzinbcba.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pjcspvap.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drhpkall.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uentceha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dyobnmcc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtyzdoqx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rzhininy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjtaxt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mikryqja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2stdsqmdz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pnnrjnne.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hfwhtzeg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rkmycisa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gduiqmod.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2opukhxal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nrgraaoa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bexizjbp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ryhyigpe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vdedsgso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edyiibtk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gburqhku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsmiebgp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nzgkekmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xllirvjb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcdcpfhh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pbiqmqvk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xcqdzpwd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khqkfjfl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2oqogavvr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mkbbgsdl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpzrqi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mltdbssd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2phrenzen.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrhtvfft.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyzulugh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sowjvlff.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rupdkgoj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2tozxffnl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2raclemdy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2flxyigqj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2njnijsea.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2umvwrcjc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jnqwgjyw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zqodngoo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rctnjrmd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lmnwzysn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xkrgtjuk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gcwmntpg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kzadqauh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fpdjgnml.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2awqkzcjk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhuxmlq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nhmnycdh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ganrwiwg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nfyaqsaq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jtwnckwx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zhkkumdc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hnildjzc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fjrdimpo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hfwnkery.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ucuwwwxi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2slrdwsgs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mheknjkx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzdrcpsy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zddlyypk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxixgdgn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rflbglcr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xmulhgfw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pjjqkecz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azupgaxs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfwlhjzg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rehupstj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cegyykqf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eogmzier.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sgcmfvie.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wofiybke.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vewxjemk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2imwmwybn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gerffvvb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zfrablym.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dltodrjf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tkditecv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2druwrsnf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qdrlosln.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bdttevfi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qzaluvay.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mcahmvhb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttrprukb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mmecdgst.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqqoluif.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewdaknpu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kcnfeqpz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dyvnhtqz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlpqpvun.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rwvrjtpc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dsvvsbls.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpxpqpsi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lxjigasa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvezszgg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2urfmnkzw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wleyvqzj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sxgcdtps.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qhximjqx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2amajzhhl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qnrwdbcz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2goufcrpg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mcwqvkdo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qjpyxjub.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tbjvetsa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vciyhqdr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vfqrqgzj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uifinvrp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yqqbytdc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2quwvblrm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mopymnkf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2puqcuecc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vxocdwlh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhupqzy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ytlytpwh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kpaeqnmg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dvibkqsa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zekesaib.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2obvkvhns.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwflqa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opnofvqp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fescwlnu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mfzvspmt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qcawpbzq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cvkzzrml.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qzjvqhku.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zcnsnhil.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kxuzzfzn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kthvhcyj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hmetfomb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2twcsharn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tptlqbun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2txehrvjv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2oiowcdaz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yacwyfou.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ahoqcayd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tabxytlc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mutpoyub.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mhgpatwa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fjeqxsod.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igcjmjpi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dxuyozpk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mwxnpxol.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ldnhaguy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tustbusi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vmvwazsz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vusgiotj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tsmitpxt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qufrjtaf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjodiko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dwfsrjhx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cwqligty.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozvtoxbh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qejuajgw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qaktqglm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ahrmasxp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtygrllz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yelzoywi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2caxflfjn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zrrzrxev.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xwwkyhya.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pnnhyohm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dadrmeet.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2msinkzgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmombddf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2npfrvlgq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fwdqpnyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhnudmdg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ttizfwnd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2atvdtkou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmpfzuss.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ngltwqld.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzbeysus.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fvousnek.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qbyffkfs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pydjtctb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpjucypl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dsuisiji.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2azxhyyss.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgmaunmt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ikciscjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2aevqewwe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhtkhbjn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ruljlooi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kznrblyb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2egvgkshz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbhvnghu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ayapsdqe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmkbmwgw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ifknoicd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rpdqnpya.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yjcpafdb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qlgoztkn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wwydusdf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rpbvldel.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2glniwrha.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2khuyqnmq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hffsefsa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vrssikvz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zzrbodgf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvorjmpq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ciapnppx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yatexjab.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qimvvhcm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ffeehkwr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cupsuxxq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2isicyvid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pfyeyems.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rxiusmpw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzhqnqlr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vxtrncwq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2lncljpbt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lhkkmpww.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lwbzvapu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vbsiesst.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xgmqqxiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qiifqeel.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2iorldnce.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ynztkamt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2prfakfct.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2btcsyscn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrcsdofs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fjmtqrpc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sqhmzirk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mvqxrjpo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rhowstia.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2unycxqar.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cbcrhncv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tfjtgohw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xijfesni.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2niunpsvj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2iqeygugq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bnibbseq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bppzbvlh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zghekvdf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rzulnphp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2eencaklj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cpiyfkpj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2myvsngor.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nwaepcsw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2uqszyjzs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2rcukazqb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hxwjozlw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bkyzexza.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lqduqqqh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zautbjjq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2uigvekdv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kijbswap.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eiwgfmqn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2clpvsfkv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2skhmnchp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kgiyavcw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nvxexwtj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2alumxrsi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfvmcezz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdchybra.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kmgkyima.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsfkqcok.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zmeclzrx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jetioufz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xukxsunf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zwzfmmvb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyukcsdj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ospnprtr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jdehgnyx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qerdhndc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ejpnbikr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bnkmqhsj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2merysmov.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2eqziykxo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ldlqyezz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bkxzyyvd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckoduidx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwryewjo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2awqncrxg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vrzoifni.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2akujeexg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwbnsur.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nudvdakd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2skgqxnaw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2rrsnmbjc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qjasqmoa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cktwoiax.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2touumxtn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hvjqdcwq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2scotqanm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfwssnw.html


<!-- 参考信息 -->