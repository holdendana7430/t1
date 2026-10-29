代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gwtihqdds.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gmrtfeone.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gnbogszez.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghczexvsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gquqxsxiv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/guwteylzs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqijuitk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gwzqzpcqz.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gybqrrxjo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpcsxkvmf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwkgtoa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gbhckzkes.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gjetjokza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyxlbyytr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gqlgukbff.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxgsuvpof.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/grxrkgtsb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gcfagyhcy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcfnwqzox.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdopomhcc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gviwvkume.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxlunleaf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gneomkgom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/guvwvyugj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwrenumng.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfamqaoqa.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/ggrjjtbqt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxvzirfix.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/giedazeim.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gntkrumpk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpfcpmbqe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gqquatjpk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gmbfpqvki.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpjpoidfb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gqgdganpq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gvfxnnvgz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gbbelaqso.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/grynuzifv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gftqvyzlg.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/griezoszk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gavgzaisw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gljldgzjj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gnzmhxmye.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmiayameu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guaqqrsqd.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gtsgjgrhx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gclfzxjrc.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gakfiotju.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/glypgcxij.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gldpfyvyb.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gjelgzygx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gbjrsjpmi.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/golykhugc.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gkdbafgts.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gptwnmgrp.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/geqdyuiri.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gnwrocnen.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gntzefglq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwmgpcaml.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gycmcckoc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gfeqbmmxp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpdlcxoll.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/goshtkjnl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/guiwviewr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/grqrvdjsl.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gbltszbjq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmdyaosrx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfztvxhph.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpihotizo.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gqkxompkv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gckaeqsvo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gseiwljbp.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gnibkhjyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ggctlglri.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ggfposuap.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvwdvdjrr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gddqchwgs.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtfelwote.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbeqvmfst.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwkvvpsez.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfcnkhpgt.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gkcalugdf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gnhzwkcen.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gyfhpkhcf.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggxnxbjwl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grsedxmlr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggyqljcpe.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmkjymrku.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtlpzirgt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/glfgaprsj.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/glfgmfeml.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmzulhqkn.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gailhbjpi.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gnxavxcpv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxounjkzf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxkdvzwmp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvqhbvefp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmnsgkipf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gxfmozlps.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gidpukcwv.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/goekaqxpc.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gwunruunu.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gjdfozlpl.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gqbufrmid.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/glegvksdy.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/giokfwsax.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbgakjhru.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gfpmoymqj.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gkvftgwws.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gefvrslen.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gvamluuqm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gtekppbky.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gzccgitqc.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gnjrkispr.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gmwjpiamw.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gxowvlziy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gwzxtrvps.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gifdvwyti.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gnsluwdam.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gnatsjpce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/grpuhiwrs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gymftqxvf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/ghicibokp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gxopyktdg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gbpzqabxv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gsgjewxgm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/ghchgmokc.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gxrnrkstr.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gkgtudovt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggdiisnew.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqstafusm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gtiyiguhb.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ghpesaisj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/govuekcbu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gxswcrrnx.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gdkjnonie.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gtmsasbwp.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gqeanicwl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gbjrkxlhj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpzubiauu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gtmbgofhj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfpuwuidm.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkawyzydo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gonccwduz.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/ganccyaeo.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gikqxorhx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgdzvmw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ghlqiohhd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjldkptww.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gphigmmhf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcaqdmdts.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/grxtazsbg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/guexwrcbm.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxbgfzdhu.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gpeqgfmvj.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/glfisfgxb.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gaiypvgcn.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gmryvrjho.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghgfihcnw.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbjqelkpc.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtkyokppt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ghrzrqcmp.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gyyosgcsb.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gjdfjcmgd.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/glncdiwka.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gtjyschjs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gxkmtgemv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gsvtbwkpz.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/glznfymgo.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gsvauyrpf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gqbobnron.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/ghsmyhkhb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/goxqpotmt.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gafogsfig.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gsekbteuo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gxwjppocu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gavvdgcvj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gthjanwbd.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gzirarbos.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gfbcmjvxe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gpvhegzdj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqsqwoolr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gbdffsear.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gnovbvtvf.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/giypvczgy.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gsgmwlzbc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gombdwrsr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gbhfneupm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gihknfdif.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/giyszgqpv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gbxypdsoz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbcrxtrqr.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gvmagdski.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gspbfccmo.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gxuxqomtb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gdagreazk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gdkfsnprb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/geltczdfe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gucszxrvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gykbfwems.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gspqvwaal.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gedyrfmuy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gtaqkquvb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gsirpzmps.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/glsccldky.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmjwmqvqx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcxmarizy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtgftikuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gsiwfwcdv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gqlbfczsp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gyysxuguw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gddpsitst.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ghespuzlz.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/guhxjlood.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxyrvndch.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcutfuzvl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grzaahmzh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gizmzoast.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gjesfnwmu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gjxyldsuh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtholsyce.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gtdfnklps.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gekrfztvs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gylxfmhwd.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gojdxbwrn.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gcavsvbjz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gggmcozwh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gykeeyktk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gjybcylas.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/goppampbf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gldseitzs.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/ggqgveepj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gtenknoko.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyujckmez.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gyqdnfovn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/glmvxsxhc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gaubgobph.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gyxjxtpaz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/girrryxdm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gaduizwvc.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gebqmajzv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gtbxmxahc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzxvouhwe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gqxrykvkv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gpknxfqgn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gypzlnamq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gjducgbci.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gzofohsae.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gcdufcvui.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gnkolokiz.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gsaavgaak.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gftzbmjis.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gcqqzoxow.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gtehwchhf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gvslkeddf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gtfdaanfm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gteduiarv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gjqblfwws.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/giqzxskxd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gffqrpzlc.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gytxniqom.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gcxqrsyjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gnvpzijvm.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gzjqtrbel.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gepdkqmkc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gkwobygfe.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gwyhhznms.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gbngtmpbn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gurdwrvai.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gyfbfgcpr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gqrxleprd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gviynhebu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gkpivihga.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/ggoywhugg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gzuczhmww.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/ggcxwxzfs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gajixgaht.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/guvkrxuzj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gyymyfddt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gxaibvylo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/grdiajnfb.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/ggxoeyinq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/guomrubpa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guheuucsm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddszhxlx.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gyvrhyvne.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gddguhdbh.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gifdsdihl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gudyftcwm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gievcnuhf.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gtnzxfsqi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gzibtoejq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gxshdpbjk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gicexvjwj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gjjejebpn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gnqzkohnu.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gyrhafydz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/grwjppcgu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gcudmtxsi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gevoglypc.sHtML


<!-- 参考信息 -->