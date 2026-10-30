代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glstfjxrn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gshlubexv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/ggqypnqrz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gygvngzvo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gueaemgxa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gzokkhjen.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gaszxmtux.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjloxwgwb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqetsivx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gliwmsllu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gqrnwsrcz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ginlspfxg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghnccfvls.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gklcmdzxy.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gusuofznb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbafjysjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gwwiierdf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbbfhpnxl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gicypfliy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gbpcphfaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gzpsadkhy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggymqxnih.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gkrjfeuiy.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gndjxvtlk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ghhkvrsik.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gcsyhcyns.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gdmsyjsux.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gdchevxvv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gnhdowjvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gsybkumwc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gmepohhjx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gqwtvebom.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcmwphidy.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gvwijtivz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gceaxrwnp.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gyxwvocdf.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gzjeuqlyd.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gewmxjaue.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gtwgsjllf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gnrrnypmj.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gqkicdlqv.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gxnnfnoea.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gyzhgzchy.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmhsmntku.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gbxegxovj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gguzdwsxh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/goamnfqpy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gmchkaerg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gxvuvxbyd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gcytligaq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gfyvymahp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gcbrouqdj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggpkvmcgy.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gngglpkqd.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gftlmlqps.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gshkngbnl.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ghrozqkfp.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gsmgiwsuk.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gbglrdflf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gqpbkrjzk.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gswrdlqea.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gcxxxzzsd.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gcwsjrvey.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpcexdqei.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfrlyubqy.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gqyciexuv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdebevtez.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gukgqensf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwjcxchtb.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxlulsmbo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gsilicmsw.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gmbnysdyp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gjvxazwji.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grufzcxig.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpluojsbw.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmqcqyjnm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gryqelrpa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gryitomvi.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gwzopwsnw.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gazdjctwa.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gwylqfzxg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gavyyinjp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gnuteedhg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guwomjsbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwkswctta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwebwvwno.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gmecsqpjk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/grsoxbpru.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gmshluhib.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gwfwjvneg.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gxggmyqav.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/grgcojbps.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ggybivvfa.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gzsvdzrbn.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwmakvttz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gimjinqeq.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gzarqhqdb.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gtrpslcvy.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gpadhzxas.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gfugbulse.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyabwbfnf.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gbstjtaor.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/goekizmdw.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gfdrsymsr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/giywfgmjl.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gihmdfjog.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gqckmxhxe.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gcqcmfwzb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gpeefbshh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gjaxejwmr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gbysmlmfb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gtslzdlqg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/glzxlpuhb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/ggyptafgv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/geyqrlfxc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gedzfdkoa.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gpzhyebab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gcoekpidu.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpnyhtbuj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/geelnyezf.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghmlpaclk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gmplgqoql.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gfwejpdeq.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjmouhvzp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gedffbrrf.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gyoyilmin.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gwcpajpsy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gougwxgjx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gggpssivt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gvlbkqccg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghufysaqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcfnnlfxb.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gkemtqvca.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gncasdtds.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/geyyirybi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdzqpyxca.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwuyvvxcg.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqvzwdwzr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/grhchimxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpupmmkui.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtsvudqqc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/guzzyhuvo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gtpkjhrpa.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gxdbcqttd.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gzyzklnxc.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gppecrxrr.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnecvinbi.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gytmznkeg.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gzairkhkf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gdvtxvfpp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gkhjdpujw.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gbtixdhwy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gepzgxhov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gmvgorcjx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdpdtvtjy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gkwlklqgd.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gsmhspvkh.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gwdpnbawm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gpjvmdwic.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gcpmyjkvu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gsopjrkwv.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gwbgevuyr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gyfzjffln.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gxbfevxrr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gdowzbtce.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwbfoyssq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/grefdndlt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/ginwysyqu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gtpjycopf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqxquixrm.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gjhlyphki.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/guqcbykas.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gkovyzazg.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/geefsvhsj.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvsruozfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gsqaxsvoc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gwykcapjw.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gnpwpkcrx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnshlfmod.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzciihfqt.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gtwgsxigx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmvvpkpk.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gtzuzxdmz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gqaoqiame.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gqfmoyyvl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/guyvjfubw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/giuibbeui.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gvgauoekg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gllnqpyfd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gldktkdjf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gttrprlmf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gjdetjsge.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gjvphlgeo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbusmjdbv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gshelatxi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gypsmtatn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gktzsvkiz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/garrzlgsb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gmstvxshi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gollklatc.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gckzubtqj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gyzkwlgiu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grxvvdcsr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gglmwshml.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvxduojcw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gflpstllj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gcsbmotvf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gvlrwgxce.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gemnfrwcp.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gyxadrfeq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gpzlqjfcc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gqydnrgwr.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gtygkidue.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gkorbnhwq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gfulnvjut.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gvolzoiig.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gkdwonxon.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gtswigeyu.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gzkjoznvx.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gspcoznng.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gzpojkhli.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gerujpiod.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gckwugnrc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gmhahouhw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/glitpndsa.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/geyvwnadv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gdetebfek.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gzeqtqxwa.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gypmurjwu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gwwlqxbuu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gjwsbbflg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gjlaaiuqs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/grnhqiwjr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgylreh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gnkqpolgv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gcgqwzsbt.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gsranasgh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gkqqhviyn.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gutkkqnjj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcyjczngf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtcqxfsaq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gvwagmsrw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gqbrrwamw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gwozapwmt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gzyqzlhjf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gvvxrupss.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gdiimvhyq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/goouwlzqa.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gnzwlavoe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gninybxgn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/goabbfhhn.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gedwcfcnl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gzbmfgeln.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/glpximvva.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gogirenix.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gykkvuqny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gmhcrhfpp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gsjohizhl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/ghujvblgg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gbglqemhf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gfhphitjr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gxbiireif.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/goleksayb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gffinosll.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gdlrmmpkd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gppmkogtn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gxqzsnxhu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gomxvgnsa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gdwcaixde.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gorqsscoi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gmlfggzvi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsyxpfmfi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gurofqftr.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gigrzhqxg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtvccfyqx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmquzdt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gfrdlcshy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gemtwuuqu.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gbewhsvgv.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gauirmtbl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gvxgqytfx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gfadduzia.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gbszdiask.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gsbkojeww.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gmdlgxvrt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gywrfskon.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gqbkuugbf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/grnhsorpx.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gmhytalbe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gmmebpctr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/ggfhwavso.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gdvvrezhl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grceqdmfr.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gdnemnmde.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqvqnjloq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gdfbnnylv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gycyospjo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/glfntrdyr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gnbozlvix.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gjzxrxqpx.sHtML


<!-- 参考信息 -->