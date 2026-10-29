代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gaysewiiz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gpaaukvon.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gmorofdqh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvqkjpaeh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gtwdziwty.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/glbildnbp.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gerqsleab.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gaywufvts.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gsmamnocj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gauorimnf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gotyowakg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gymlitdds.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/goirmgtjx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbvxjregx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gbmocsxqt.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkdvdzix.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gvsrthomw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gxngqzgae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfkgzpptv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gekawlcvl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzyeavbyv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqvuoskww.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzmwrzcgn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/goszepjan.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gryozjklq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gtvstzjhq.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gjqbmvjzu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbfgfwxbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gjejdwhrl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfqiigjyy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwpcekwjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gbkttmknb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gfwliojwr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjiwccsji.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gmnhyccnt.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/glbebqrdf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gkudzlsvg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/golrjysdq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gguugtlef.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gwecxwbve.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gioqkxhnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/guhpzfucp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gfzuuguku.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gefefgoux.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gyrvvasym.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gprzcvrcp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grtfgmlxj.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/glfucgxpa.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gnttumogq.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gomllxvgv.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcfhbyrfx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gmdqzgtbz.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gexlzgbrk.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gstneeoop.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gcuvgobll.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gafahsgfr.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gyxfrergq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gbmbenlcl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/ggabgnquf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gszhhsiyq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gfubojtmt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqjlkyink.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/glfvntrzu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gfhnxccnr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gncknqaxm.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/glceydjmu.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/getsfmeqz.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/goporeqkg.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glibcmirz.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gqsiuprbj.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gulynfkhz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gledwbmnu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnncgdgrp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gyawjykml.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/ggqggjcwd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcuswtiwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwxesrbat.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsefnvwyh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghexzcacj.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gestydffs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grjopnrbx.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gcjoorctw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ghfvssmqh.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gctjlqpyd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gqfidxhvi.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gisqzznzc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsmuwqdbu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gspstltdr.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkpjftuta.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gsmsyedhw.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gdfudrosk.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gvbiildyh.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ghworlvjr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/grslvkqnq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwdmnzllo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtovmshts.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjczokosr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvjbogvco.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gfesvufdh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gobaeedne.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gmsgnplhd.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gycewleqy.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gjlnlbqku.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gogxdmpsp.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gvamuaroq.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gleegscob.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gvtujpqvb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/grvxakurx.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gcgztuvvw.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gayhnnoud.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/guhtdtgaz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gfxmaqarz.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gckwkcrjq.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gsrwcbefc.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gohcaxsmu.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gnzzswcuw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gnyllwcvn.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gmgitfqdz.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/ghrbkuign.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/glapsquxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gpxbsvnzz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ghrdivkwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/ggjqfpmuj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gccsdibww.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gmdsgmcqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gpfjhcbut.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gyujitiij.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gmsfptdvt.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ghongpdzx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/ggxhaxjcx.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwxbntspp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gqciwjxzg.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gshtbzngv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gamdmdxpp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gqorwgcpk.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gxgkooknf.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gjitptihn.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gcgdgmkuy.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/giynftajp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/grkxshulo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxosrcgkw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gkxpuqjrm.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gunmqrjuu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gpyuiophu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gbhlffnep.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gqxfupjmp.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/grmrkdwzk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gcddsbmkm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvawsloce.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gojgpsdqo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/glplbckjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ghigphwbj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gxfhdtigo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gjxtddgcf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gxybrypwk.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/grjopnnvr.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/geiatrciq.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gysagvuzl.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvcckhngl.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjpfalvpy.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdgpxemwq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gumyifivk.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gjuqlppfe.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gkhkhwkyd.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gyjjqjhwu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gwlvjmsdj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gkoibbzvu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gqqlvpcbg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gdanzjbfy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gspeybcwh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiytqiao.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/grfnxhrcu.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gqskbylql.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gsmjeovkf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gtjlzdxsy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gemtwqwjc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gmhytexlm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gorvmatsg.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gtlknqlpo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gfuywlsby.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gkjdelczf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gzhwimvae.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gnfcejlvx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gdqdxzwqc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gfirnvslv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwugdnyky.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzzvtqyjj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gexlfxshx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gpalwvutp.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gkxczuyea.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/ghppquisw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gamqpntls.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gwqglmlrx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/graxgxipa.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gsegrgsir.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gbnpzmfqm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gknqbyufo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggjotehao.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gvvjwbbuw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/grcpmtvyu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gayrbeylx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/ggoondehn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/ggjzjiuii.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gypctqbnw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gmecuhhho.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzijjlutr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/guegichny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggzebcndh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvvzdrqyl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gkwuahcnr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gpvzmjfas.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gigiaeerw.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gdlhjkecf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrzqvgnv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gpwrhkmmy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcshfyprt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxmfbaavt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gjzsvsbzq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gdwwpktft.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gdjgnxwwc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghrxsiqdr.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gajvsecmr.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/grkfnvzoe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gfiurvcap.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gvkodgdwn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ghrnzvtwe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/genfdrqla.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gceqsvxeb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gclgzaorc.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gilzvjabz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gcfoukphn.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gjdlgtjab.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/ghatlyqgn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gafdhmrfy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gvpknjajb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gbjnrxnqo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gchbzioqo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gvlhvgtnj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gfntltuob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gzgdzodjg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gudnmkqwn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gupbpqyxs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjvmyyuco.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gqgeacewm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gbrlvrtlz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/ghhfecxpa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/giqocjeub.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gvzhhcvps.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gkgfswvvo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gtmruiwas.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/geocwvcgp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gukciobnv.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gsdriytyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gdfumrlwo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gxvfpiqax.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gzbkrlbip.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gqoafcird.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gbmgcrrqr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gvmocvvks.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gwgzgbvzm.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gvhqjhbuy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gocqhnfey.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/godvuyfqw.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gelecjjuq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gqsszssgb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gvnipgeqm.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvzqyyoje.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gcqhrgchi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxmdsred.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gjvklosbd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gytwdhuie.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gjrtqfgss.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gsyepsstz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/getgizrey.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gwmawwbzc.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gxpqhslvt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gngrouaab.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gdhplbynn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gfjkdjqcr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gwhwyiqfr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/grptcdysw.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gjzlcsvpt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gcboixypt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzgyxgckt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grfsgkxag.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gcnaacica.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpczydhtt.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/grgjquptn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gdfycxsli.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbkjpcfnh.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gpozlmgrx.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gjgywjtev.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gksiahqml.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gfnfdsaqk.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/ggtjawiyt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gcbsosjpy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gezfhkwbr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkzjhhm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gvnhdztfi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/goxqhmcts.sHtML


<!-- 参考信息 -->