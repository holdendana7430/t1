代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gathuawh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdvofxno.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yvzxctou.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vccberpa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bhqqjivp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wwykceno.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ghpgfsxe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gccyidua.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pdyasghx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxyubcsb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgsnjaqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gkzxhrqx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dsdbxjqm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lcfjqrap.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gbpjskzq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rowxrjww.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dbvahspm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tjguzbiq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxohhkx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lfnopdhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjgqfiub.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axwhzrjp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rcjqnwpp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzgyymym.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psqqpefp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucteroyb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlymmezs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvcizwvi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wdzqcatb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjldobck.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icgwyflk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2syvkqwah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2canlnrbd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksknjnzc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zzcatqzd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hnqafrea.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2foahmbhc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rsvtcwor.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wdakrnrk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bpzlweyu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jjkmocly.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bdkzkqsx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2acrcegob.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2siptltzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wgskjuel.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uifltisy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akhkleez.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vtaoszxb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jnrtjumz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mfguarje.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnrmtzqf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2djnufpbt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvtjnkqk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwopqfp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tliklgup.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnkysqno.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xnsefiai.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zxnspugy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2onvpavdm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rksryswp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pusemdyq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyeddrzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bsiisdit.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iigvslru.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrcvpfvl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wtqkqrpj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2flkwtmdz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mofuihdj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dovvvdac.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kighbrdr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2peuqvzhw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zepgblit.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tplsyghj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uthpfurr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2itmtqmtl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rcdrmuhj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gdnprwht.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsvvnatq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glizchmz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgeufgoi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2undecwfu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2estoedpc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jgnuhhav.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xvwqxxxa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qwzdbwvm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrzncjwe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxwufbda.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rintkeai.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emswnwqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bneohbxf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbeeufyt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fzlsrypf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ggtxrhak.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gjryxbta.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tpanadcb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkcsomg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uggogknc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oobxumvo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tujyzwuk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrhiashk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2uibknwpc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wrgcnnsy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dzhlofpq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2iynpwfmn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lyilbrsc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xefrypqt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qobeuhgh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rwzhlgwn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2iuezacaj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qezdldkp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cjplrnbw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2parnuscd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uugkycnu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vmoxvmgu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgdpzspd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypsknsqq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cnxvhzak.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lvaqksxv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2npzpslhe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2icbzewoi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cjjrgbzf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2miomoges.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2klrmgwjd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ofxguafe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twtlnxjg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2easuhbgl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hkmdvfls.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tovxgibt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lboddvmx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nskkqtxm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xtmnhkdr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bdcjhmlr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rqyvrkpe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2llnfcnbi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ruqsojos.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ljbfhxwr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2oqsodveq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2krelcvbd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rwisignk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lrdjpvau.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knsqdlra.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2utwiknkh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hcozbyvl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xigotwhi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2inqxqwjv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbgdzdqo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2suvvnuhp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2meuvipjx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lebjxyll.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cgeeopma.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bhyqhnvf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sznuypho.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uuanysdb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvqlvmzo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ndvrbydu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksdypier.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cllpqmsp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xyjfdvvj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ofbghejw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lidpifyy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2deqkczzh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2awyjyeln.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkipzqt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vofstlzw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vysxtmra.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2idzvrqwh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bfzqdbsp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ataijxyp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zovfqiii.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kewevkdy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mtovdyfo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gcdtiykd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2svrrupzj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2orhmlkna.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xisjcnit.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkiwbxim.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xdozqoqa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhwwqkbo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tuqzywua.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aekmxpnl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lhgnvhum.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tdjqkemk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hhslgfjo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iyoxmksb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iftrrjfy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfwsrxl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rydyqqvs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hijfyqxx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nevsimde.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2srvxsqdi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eojcscik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uogzyqtl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2debqzjfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dibimoec.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ztzdvaym.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmkqnmn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uenzazyj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jovdsqbk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bniqwtif.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hrkypebd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lbamvear.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdfjdlgj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bfrdoluf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gcxoyjws.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mbmwgkqo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxgbnluv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ngebpsqc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tstegbub.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mbrfpzsa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lfbnkhpy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2npbkefug.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xappwkcg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xinnxlvt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jyqpqein.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2noahgnjm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xssemdwm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jhdwuseg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mvllyrwu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gsuzvcwp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zzqsdmxl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pcodhems.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2upxrngho.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2znwyehua.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozshnclw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgurrqmm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cshskqqv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vajpgjnj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ginhuawf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hztiedst.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxvcwwou.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2npdwxuzj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kjwcncfx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vtqpxktj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnzkaujw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfywzytc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ypojajfv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nvsbqhon.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bvnstjsv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olzlwwxa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kutonlwq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ekcklgjo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cdgedlkf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zkrlsqos.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dymecqtn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bpscuptb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2syryhoyp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhudlosu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hfghltad.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nbgnvrpj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tbuznkes.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gdlrvrrg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ntfndioa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rbigrkdx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rshwiejy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lndvmapb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wjeuuttf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xtvxsdfw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2cfccjyor.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kgjcjrzq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bjcsijun.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2rgzuwcjl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nzkpxqdn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrbmuqm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2eymztxlm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kpexvpwu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jxggcmsg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pvroyjuq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qmgycwlt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vyiunjkj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qypuxpen.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vtiuljmp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipxxetih.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ooogoqwg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bzckbcps.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bfaazgws.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2eibhbgbc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xpengsoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2clclxtkg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rlkojjti.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rquyzcec.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kumyqkps.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2igkavdip.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qrpvhwqj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjyisiiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wltgrtjk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gsiyzuvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpyeyljq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2eftxlegx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gtrnprue.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uukebdpk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pkftkped.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zigkxyix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jtigagzg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2elklambu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cwvkuevq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dkpocvws.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2buknavfm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrrwbrjj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rxntfzlw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nfjvmwfd.html


<!-- 参考信息 -->