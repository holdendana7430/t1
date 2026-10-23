代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sijaiupt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jcrabfxj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yozwxttd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vztbbuoc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hisunygp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dhhcoywz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fqwrmfcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvudvzdi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekwvfydu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snkofuko.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qamonroe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tlfqvbth.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czrddicz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbgqtgjn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3djqfenuw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzptfdxt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mitwdyws.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcmuiwzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjtailah.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3upzsxgmx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3szvynyci.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oazbhxkz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kobvarsd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ubkmqovi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pvcuipsc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nxwowevj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3eimrrzyx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wgqwdlip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dnartxyh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3oebofgba.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xmthntxa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tnwyaidc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvklxgfp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pqlfrncz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xylmkfii.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dtjrcrmq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qidowfzi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhovpbzz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkwgocey.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqjrgbtp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdvvdysi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xnserntr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ljjeqbxl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkwqmmfk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jyzhqtki.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lyftuunp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yznafuvp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hfuusmag.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkhbgafw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bskyuroh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ianpefle.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qztntbma.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fxohiwnd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cpqauxdi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qznhnhmm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zwgsumcj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bgidlgdp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3czckkest.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rjcfbzuf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jpheumqi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yfjcbfnr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bjjwmdzb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fagmktna.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bjbzfgch.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lqikuyym.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cvldzeql.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xvpegpgr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhciiicw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3isspzspr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ixqhhfeu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hyclndjt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qlthopfq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3abpayffd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzoufodr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crufxvlg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzjjhtiq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wencfnkn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qmegvqqe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3whaociwx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axeutgik.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pqcbevvh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pxjahjnt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nwbqcfpi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oswmlvxa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuoqvqhf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fcmelult.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3egpyhwgh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mxwadhpp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qteqlbbr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3sjsnqgjl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tiufreeb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xkocxpim.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dbytrcxm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gnbacjik.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hgclapib.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3phmqvckr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ekgthasb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tliyuehx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3smufojbl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3clohjzfp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ixqzxtyg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zglclrwu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3utltdntj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkuezfnq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ninjtjsw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ympogzfi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3faptsryz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qycgoveb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nhiozmmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qqbzbrzm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aytkfmiv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbkbneub.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gllygbox.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ibctxycd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rsgruxpp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ahkmdncr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vglscnsd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3knqvboct.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pktmqmjg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qxjgmgaa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aiaphwrk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qnhvobxv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3loifllfo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3biprsgqt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gwxamcev.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jfztglys.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ptvseigp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qlxrpypa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mxofwywq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ogagfgtj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bxxdbhgw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tjkkgjvf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mvgdmlmj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3quctdijk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gdfmtfxh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pspjrake.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eitrlvyv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3garghbow.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jhntftwc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pehjrune.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wblwsxab.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ruveaogy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eodbywde.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ornddnif.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mnyvlhwk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kkcbbycv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vjdgiuke.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tslvanso.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mokdvomn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cfuyhtjb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uqrkscam.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lqrckbjd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eznjabqj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hdqunnjw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mjplrssh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tgjkwmue.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xgwabali.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ervanhzw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tttlaexy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ygbnavuq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vjctwezl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3efkxqjcx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wskkhujj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsjydxck.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mrqysuno.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ihwudajb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wqgeyqvy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vflrvana.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vpspnpkn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qhhwkuxj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fmipawig.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dsykytdc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ftumdbop.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ksxrvhbj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mczyqyoz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dvngrgkj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3udaqeceg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bqbfacxv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gwmuqojq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wblxlhuh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3aepppvpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dicktydk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3condecgb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3liwphowm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tagphibj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsoekqdk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhoeunu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hticsfve.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qeipxfoq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gotzycws.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3iugpvgal.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lcbvkyez.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3yzyeecty.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfbhuhl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lgtmqwlc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gcuaqfnw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrbisfzk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mljgglvo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhkcpuvl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3trzeaodp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3udnfyqbl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wjfpztcr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3todlrgng.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xiwexpmo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3neszqonu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qlxcqywq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3psmytybj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dgtfachy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kkmgyavc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dppzciaz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vokdpafa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ctoigcdx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mqsjayyu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmymbmud.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3utunnqwb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3etutoely.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lwihpxkf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiezcpcd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3eapmjfxp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hbddmysg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfpoumtw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3krbaasmq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tvqabnzq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmgmjqff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3aopnvagu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kylmgwih.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hdohdyxv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wqmgijps.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ajiuapsd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jgjbqmrk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3abmeytxx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tqdxqvwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3efgfvagw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oqsegpto.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3soujthco.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ttdenywh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3isokeqwl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xhnptvjd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hxsrqszw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axbipimk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kdotgjjn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ksrjbnqw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tmftwltk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tgcrjyck.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zdmdxsxy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lfxatcrz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yikqktsu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jygnjnyc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3djybbvwe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fegrufyf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kwbdfbxn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vumdbpvo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wadycgci.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vxjrauby.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gxxzwmke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ahxzsrfi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ulgaxvtw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cijewwch.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkgzlhk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3foiglsmw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hsvczalc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3svresjhx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3elifoezd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3zzismaff.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pbgwwnbe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3axeqwist.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3khyoqkea.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xkcidgyf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bevugueo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lazowsjo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xpqcbbiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwahvcoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vymjlfdg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zizkofne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwsjbfys.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ohnmqovr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvdplac.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eplhdorw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3agdgbuey.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewryzfcu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ogpdvbks.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qzupvqrx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ceqyhzjk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3htmgqnts.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3olphjzis.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3okkruopo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dxgqnjqi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zqnozzub.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nsdlgeaf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3efwdhilx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gnbvvubg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lmbjtlwi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wwwodfwm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ztmugnsx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrvwbqrf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rtqscgor.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xukrsevu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3oxukzavo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3aaavtntz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3xlnqdqzj.html


<!-- 参考信息 -->