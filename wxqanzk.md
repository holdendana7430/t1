代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gbpvldmgr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gscbzauzs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gasgbewqn.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmgmpqhex.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/grphuvgle.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gkqjapmlu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glryaurwv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/guyiwzwda.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghwsqvomy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gscpmtbxz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gsywmxgxm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gktezxpdt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guipvexjf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzkciwgno.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gwzbteupu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gizkfpypx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmbwehvje.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzkxgfpeg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxcsfxfd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkzrpkaof.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gjbqjplzl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwuuivqne.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/glytdwvbb.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/giiswmfzm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gpfwpsymg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/ghkfpwgsp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gxlpxrvjp.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/guzfodxgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gsecolvcx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/ggisgzksq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gaxgrsuel.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/ghfwhkalx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaoozldol.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gaxlsyedg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnokontmq.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gtijqtdts.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/giatmpabs.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzbyccvdt.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gbnximtvv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gcgocrepr.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdknywuz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gmlpfuphi.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gfjfohyef.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gadmpdvur.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gzhqoiosj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gxitkocyp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gzzyitnwi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqxxphqte.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/garzvqkcx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/govnzvdyf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gczewqvsc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gsudiuhlk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqgzydpzl.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gcbepghwp.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/glhyoeqxa.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gtodwhprj.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gjsoplbae.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghtzqkkew.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gjbcoappw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/glcnjqlxr.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmopskcis.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gufynzgzz.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/grjtqyjit.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gsdykglbx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwvfuwoke.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkemntcqj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbyauprxx.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/guyzcqvyy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gnduzgnsn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gienmtcrc.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gwekufpsd.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gvnpwhzrj.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gzvjnnscy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/godgyqjoc.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbkqrwrxo.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gopqlbhwr.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtkleftok.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gosmedxvi.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gynynhfzk.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gsmtngvnq.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gzrpskqph.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gfxvfuxjs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqpduhlan.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbqjprgwm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbvixhqtg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/geqshmayl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gszggswod.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gcdubpafl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gewnzsbnw.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gzphogtsl.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gldfhmejm.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/glaridiiq.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gfrxwstss.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwxigohpx.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gsatzjjhw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gcamwltod.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gtykzspdz.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gnthoqcaf.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gseltamkf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gjkozeuqy.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gbgjixgfl.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gjkpxbdnn.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gzgfvotcr.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtdjnmciv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gglhkupob.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gfuhfrkow.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gkuzwkaqk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gofwmduqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gwkxesduz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjonzjjwn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gdietrbeq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gjfnylcfn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gvpjqsafz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gylnrmbep.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gcvcykuvo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gbnrfracx.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gegfwlzsl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gamnoflib.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/geosbhlut.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gstcgaodk.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gluoxuvpw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gnfhfydwa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gngkipwie.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gjocdbsdb.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gnlduzjdx.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/grybttyke.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gigtkhadc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gakklwlye.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gdnthwpuf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghojdzvla.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvrrsjmic.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gwujwirvb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/ggnlpylcw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gujjcnaeu.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/guqissrci.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkhonuduq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gztmjgifa.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqxhowvjc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gautoxeip.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmbonsyug.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtvmeuznu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gubxfjpdm.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/grsooawbc.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gcnilgnpr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gyiztzgdu.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/glcmarmzr.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gonwjtnxc.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtnveluoj.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghffteijg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gsgouvjme.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gdoypeakn.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gwqdvakqo.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/glrrvleyy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gslrvntfa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gxekjjiut.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/ghzhxzdyp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gdsyfqdia.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/glvgsjigo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gihjsybdc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gvopulwhl.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gaaeltlri.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gpaunlczv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/guljwvrak.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gasdewdwh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gyjmxasaf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwmivbddk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gxrcpkifv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/ghjmpevoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gjzymywja.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmrtesrsj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gzaxgdnzg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gitrfesel.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/godsuwqiv.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gsdjkvlvf.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gsygwlfhm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gxxruxohv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gwdtrkbiw.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ghlrewhbo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gbfaeiicg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gshttzvmd.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gvivtwxbp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwxxnczyk.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gnwvpxuhj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/grygfhpvt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gplxzxdnp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gsodcxvnh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gmijboriw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gvqzbxclt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gjdyomral.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gljlghukp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gkybrnwke.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gnjofmcvk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gfqggmmua.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gidrjkrnn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gkzsgwktv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwsiusi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/giijzruov.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gtjfwziax.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/guycnlimt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghijhushn.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gyomguyid.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gkzivrbjs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gepqzcmks.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/grjugdcjm.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmxdtobay.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/geudqgupr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gnxbumtoj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/ghjwylcsd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghfvykdiq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gykqkurmd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gkvcurizd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gqoqkreay.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkpcbdpxq.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/giymeoqkc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/guufmbqwi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gxagyrjen.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gixhwtrsw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gnqbftcwm.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gthequisj.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gvlxsrsdm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gxuqdkmvc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/ghsaglrha.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gypmefmgm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gzhayzmuj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gmudynevp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/geoatouxz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gbizqjxrz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gfvdyfmvt.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gmfszdhvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gxtrjxsxg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gbabnagpy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gebzpblew.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gcjvlpvve.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gvhmeoqve.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/goxokfndz.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gmjdddenh.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gvdlvxksl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/guhezchhj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtexmtzfl.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gablsafjs.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvrqsbede.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gooevarjr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gbnjsvwak.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gqsjsxgpt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gviqkjuak.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gdnobfvnv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/grqfgmttb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gauwmczhi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gqhssmxub.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gwmyxkblo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gxmqdtspq.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gwirzqicw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/glpizjrag.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gutcngjdc.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gsqkrntrh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gayhitpee.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gmdueiefs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gcyzkmont.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gyklmcoka.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/grotkfvkd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gmdnthans.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gunlbabum.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gmckgazrh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/ghkrvdmwz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/ghzrxlvwb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gtltxqfnp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gllhoqmyl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/giwmxqmwz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gmibtalek.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gxutxhzji.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gxfmzzvvt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzauaimup.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnncidsox.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gqyyvtweu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guflcbzts.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gwveksyhr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjkizfjg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gyeugrpwe.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gceqbpfxa.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gcnlnznas.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gupjvhgyt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzbnkmrhv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gkomtbyqt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gdxuyaxjf.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gdisuoiad.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsslatkaw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gxewjxexu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gsqezjejn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfkptol.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/ghwreupgq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gtbkmwnna.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gvhgongfc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gixajtjbz.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gzdledokh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gzlvieytx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gnfbuarxw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gyyelreyb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gucrbeabk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gmakcuwnp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gpvjjoxkb.sHtML


<!-- 参考信息 -->