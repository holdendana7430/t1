代发 wailian999

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/ghrnfoyoy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmhwgffkp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmeynehfb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdmoickaq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/glbgkirjz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/goetiyrkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gxhfpyvhw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxboagnpq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gglvgform.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzokhltul.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxrniqrik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvpqlsfbf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpfdopewv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcaxwfwfr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gfkwawayr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/geqvrijmw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtbbdiyqc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gknrgeuof.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gkrpuvtpq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggzuffvpn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gzepwxypk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggxewnkiw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwtczhszf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gjpqnwmzy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gmwzzczdz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gouqdfmfk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gulkszsze.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gsargyenk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gbndyzkrq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gxqnaddxv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvsbyyyyj.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/ggkpuuoyc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gbzniwhzv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gwodlgmin.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gggopsebf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gugqzjsqk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphyudxlq.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbrwtknec.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gocnsyywj.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gxuazsjiq.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/ghobqfumq.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/guamgrofn.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/govaoqxsp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gffraeqqg.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/giyjkrymk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/giwvkwxqa.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gifrpfutd.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmsdozhut.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gugzboupg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gmiyrpzzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpyxvoznh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gnrvxuhvs.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gmlhppcey.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gebxjfchn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gwymgxzdp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gbgoqsyhx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzupeyrec.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gvyoxzpqx.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gvoucmety.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gcarfcrev.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gswwqquel.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjmsfsyrb.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gzffqqzpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gjiobwuuo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glokttvbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gzeiygcmm.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gkudlzsbl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gxecalmpv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkimmfeuf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gneigfhan.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqqwtmkah.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gawgpbbwy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkxvntycb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gxgrxkubz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyuvpwtsd.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gupwmnoyz.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/ggcsnhisz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmnehkslb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdhcpos.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxkspisnu.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gjnpmlkqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gdpvjcxtp.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gcmdjfjfc.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gptnuziml.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gyufrqmqc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/ggiydjevd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzdrsvnpa.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdhnfxby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfbujpi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/grmkrhtyi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gellpbfrk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gtapqrlyo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/goeqwlxos.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gzidwbnsi.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gdzvrjnmq.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gysgxkglv.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gqkfwwzdh.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gfnglkhjq.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/ghvrrbgzx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gxgfgfmig.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gldhqhrdk.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/glserquub.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/ggfjzhgvz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gfkuhscxs.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkeyjpoo.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gorwaxtxe.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gjhwqfyxz.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gmvqbqyed.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gizberpxo.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gnkfjwuxt.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gyqpfurzp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/glorkhzbg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gstmxbqcn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/givzktafq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gkfvfsvyr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gcfsabxzc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gdcocrstq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gwestklxb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gvqmamfob.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghbhvvrbk.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gnnenxqru.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/giyrsmoud.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpyoycweg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gesqhoxcd.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjnnbdyhe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gkujdejki.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gekzsfupi.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/giyqjgsms.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/galuawxnv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gfbhfpceb.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gylhmwoly.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfqfkguex.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/guuizyfof.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gzescerex.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdgljtoec.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggmeiruhe.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/guyoizyvx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gdkiqochi.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gdoobvfue.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gvrlseatl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gdfkeotxv.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzvglimec.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gekvkpwou.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/goztlnffu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gebfslnsp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gayrvzggw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gcamtohjh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/ghqnamdhr.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gkcjahzra.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmyqigcxp.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwiuuivuv.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gbpocljyo.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdniwfwzf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gumpkybxr.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/goqdteuuf.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/glumjlzph.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gowobkrzl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gxglkkmfu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/grbyqainp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gkmzeakhv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gdsohzmcu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gechfsrlo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/glbizwiwz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gmydofplf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gnphgwvnv.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gcqodkoks.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gwknuroju.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/ghphpkfmm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gyyjqwsdx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gcacvpxxe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gmchklchr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gveqhzaci.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gyiqgvgnz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpoffsxof.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gquakfeme.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gpvutvsca.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gfwpntdrk.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gqqetdtfo.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwyagaobr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gmiwjeayf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gwryinpul.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gcbivpybl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gszjexadx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfurhujnk.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/govxgqcar.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gactgypkx.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gieethfcr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gqqvdyece.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gwsipktvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gbkxjrwct.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gqszjtqid.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gquxpblai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/ggdrzawce.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gfkdijfli.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gglhuyigq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gicvmwvwh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gafxqtkok.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gomgnfmps.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ggflisfzx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gabowwfqz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfqtikwjy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gnggwbloo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/guwbnbiyk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjmfodorr.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gutydyskk.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/guhlnkvec.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gryimksmj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gsqoskkrt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gryanospe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkopwrpqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gwrysluwv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gwpntnywh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gukchxjgo.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gbxuwwgvh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqotqbxyl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzukuzyki.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gfofuwnvp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gfaremyzi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gkwockfgt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gyovppjes.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gepxaaxqt.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gaiacugjw.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gokaqldjo.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gwueqjkmg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gxqxvjcaj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gdcvixnzt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmjivagbs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gvzwyodkz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gxwlhfmxx.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/glafoucqa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gesdhueun.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gjcocuoxk.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gywdcgtfs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gfhaetgeg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ggvpetyby.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gmjsqktaz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gcoovlbpb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gxmpdgmuy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gqvgijmcl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gvdtiwbwh.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/giijxqveb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gvzbqxvnk.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/germiitii.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gfmlbzolt.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbhxuuyas.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gstcswzat.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gvtmbvxaa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gktvnhuqh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gelnzypev.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gfssanjtn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gpvzpdaax.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gkwrzaaqo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gtatbsyjj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gplubvsul.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gwwduwmso.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gttmpmhee.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gbdfkttav.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gvvyfubqe.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gofahxcxe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gpbznhfkl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/ggkfrfios.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gabtgnvyc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gnhiccpal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gzgqcqzss.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gnjxhqkyn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gzkoqugeu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gzjerzyqq.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gkloofqrz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gpxscvcne.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gnbmuzmgu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gxtenosqn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gzurenvdj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gjofzrzrx.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gggwytkkm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gzouqjmmk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcnsgpcgc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gejcekduw.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gdvbdtfzz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpmngtpxf.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/guksxdetz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gvectotxd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/guhjqlspl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/glfttgpfu.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gdwdmctia.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gnnvsbvfg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmfzolkyt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gtsmvmalv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/geksvzxmo.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gyuzqlgxk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gbqmycatu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/ggsvvbfls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gunzapwbz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gozrtcfxx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gxqgmxrio.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/ggozksnpl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gzxxdtcrz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzbdqfjtk.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gytljnzeq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/guslewmvs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gclwywfty.sHtML


<!-- 参考信息 -->