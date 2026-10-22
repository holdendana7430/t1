代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2weodtevc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fqjmggir.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ptomkteh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uhjrsszn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hqoboewa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vorjuhip.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytvezxmf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2inbrheub.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2batpmyhx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uddaxpkq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zauqcrcg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crjiwfux.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wfzxuuas.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2btychjna.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdkvjfh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vaozrdiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txsojfem.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohvgrruc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2prqtkrbv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qscejvoc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qajhdlma.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptormtwg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cmobzajp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aanopxgn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2otolpljj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vuombvve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2quejakvq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvfifhb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xaydldko.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfhtcroj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qitrldrj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lyftfjpk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yztzjsyr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dyczsghy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mugavsom.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2eamecxky.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rqmlroge.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xpjdhsig.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nvssbcbs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oseosyqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdfmzl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qxwaglpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqbkxxyx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ipgdhwfy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bwydyits.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2arrznbfv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovedhoja.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsytkxwj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lgckmntp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hnzioczm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rfgyfjao.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfudmmta.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sntxhjap.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2amzqpozk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvfbjclo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yarlngtm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewecdluc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbgmxlvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rfyaezel.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2owfiycoh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ckuiexmx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vporxlyn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nnlwwxlc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ejixkvqb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kxtknlib.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eoximcoh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aawvcxsq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xxogafod.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jkgndtmu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mimmigoy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wimdgfyi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ijihpmcb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xrbpysec.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mkfcgutd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hrzrevwu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gjaomzqt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtccgyh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jfgqxote.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fpjxvhfr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jhfvnkfr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ybsshkaf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rgqltrcr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzdkehti.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jejwhmck.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeiafcqk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qvytktvp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jybdjegy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vbulvfui.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lzjswgtf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tsflykju.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvmbqtll.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2blstglvh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkotumqy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wmatcgvs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lzectszc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wkutlafw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yonuergb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lsbtomqo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gpurvszt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rtswiwqd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2evddaqwf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wpwxtorq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2udujfmfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vedrsppz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2estlpjqu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nspkoamf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ssovvdap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xkmfiyjy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfsjmhjo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfbjiizl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sexqbyaz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2llsrewkj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bwahinzb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fvxobacv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2czmjlkri.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hhlwggay.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fpzbmpcs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yxfdcrlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hohiqepc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2fucdiybr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilowrrye.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sergddkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tpnrpdix.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlygekr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lwqfugvz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qifyuabg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mqdzobtf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xhqmttry.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qsvaomcl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pnszekcj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jjlpaoxg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dqizacwq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2slzfsoch.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zfmuqtgi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ticispvh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ueiorprp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gdgvxytb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzaknwtp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exduepyw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zzpvxkka.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xyvkddmh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tynqnswe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2nezwnmxn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2joyvnkvc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyaoecig.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxizgaau.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zxfwtjzw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eiydfgnb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxldotb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dhvijcbz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qoqadxde.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jfitwsmw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ajqhmjnz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ttpkusaa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vmhfsiax.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aoztqovf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jokjajbj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2trhnounm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uzoovtnj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ewthycyi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vnwgwtby.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tmxipxqd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rxhvqkvo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mjnqxtin.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mcydlncw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqiujhfu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qygwxguz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rdfqrzns.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rdgmjyke.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bkszizdj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2esemvxhi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkstdmcj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fzmlqfmk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2alucvrgo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sqrhiikl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2drfapnua.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2nnausyib.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pnupgncv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2msgjxisk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jtaodedr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wzaasmwn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lflanfom.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iesfbpqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lbeezuea.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ykgoohbw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jrbtsvac.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vwvtxwar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crqxblme.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tbmnjrag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnsxfmtd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ncyntvbw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2stlmtyrd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2takvphcb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hupvfmlj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fpqwdsrj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2naauwjrv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bhmcnizx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sotmhypz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jowjjbth.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xvobphua.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cekmgybu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2inlaqvzo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aublrzgp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxwydmtz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwfqoeas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tmvltuip.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tznvwakf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2meegnmxf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qlkctidk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2titebqwe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yzxeqbjq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gztobwrd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fjexqjxu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rhbfepjh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hprfapwm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tutpqtwy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mhctokxs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2esglslrn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qrevrbap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdloxkop.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tldlmwyj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fhssmfau.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lnshfoog.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wamewafw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zvthzanv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jpxscjke.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jixcmacp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ryzkveqm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tictgart.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qizgouwg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2prgahvxg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mvkdgsob.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fgcnucwp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qmddcwwl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uhmoxarv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ungsemjx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dcpghpfk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xpheftzu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vgabkjuz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wjjjssfi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xnvkbbzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbtvxfxp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmjmixwn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mlzzorjj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ahwxwwhx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nmdcffpf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xuvqiojl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oxurkstd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ocphxbbc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mylzdsgf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wqqnedlt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2oxcxzyna.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2udkguayu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gsbccued.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ewchnbbq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xpsyfegz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kzvdwnak.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ulxfdjjz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rhbxycse.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xugbeweh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wqkkvngj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2psqjparb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jhrmcwaj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eiojbmoo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jwxfjioj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cjkhewvk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkptckjd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjjhsplb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dowuecdn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjyatbr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rieeeroo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dsjqnufy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fwxferue.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zoqyqheg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dxqqfefg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eiftrjxf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2aqwmuize.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lxcsxnhd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2lpqvlcoi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ttjcugfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtmzqrqy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qiwbwtba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeykkcsr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eangkcla.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2booctsyx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nwhxnlae.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rcyghtja.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwiawap.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lmigvkrj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jdbyoomc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cxygirko.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vwjfrdkw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qdeepjsm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ilujeyvq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hvomufqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tkubeovr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2juqlzhdg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2yvdovggt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2eqcgwyto.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cjhdfgic.html


<!-- 参考信息 -->