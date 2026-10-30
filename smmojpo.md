代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxkqerlsd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzvfpftxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gwkxwurzr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsrvdpucu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gvmamyeuh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gtriilgoz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggoxnnbgd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/guneiprmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfrtffpxw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gatjpbosq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gzmuurlkf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwnhdmjnk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gahicajxt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gshsheggx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gxnhilgyi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdyxzlutt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gjnybcrtt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gktnyntpb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwasrbgjb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gqvbgaumb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gijlllkvo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gspqyqvgc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gklefceso.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gbtkbbgrr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/glfkkfuyu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/giknsjwoj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gynakwqwh.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gqbzeofrf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gowwncvzy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gmxmistfk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gqeipiwxf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/glirgnrea.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnfzeriwv.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gszvqvpxz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbszgosaf.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gmqusiqgh.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gsnoyvzmt.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gfrmtlfqg.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwfryemdb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gvtjlxrnj.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gzymkahbr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gkqvfsadg.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/ghrgcsnrt.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdhcmihfw.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/guzehmehr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gvmihtcmb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gxjhsxjfe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwfdiosqq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gupwvdkgy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gldnzhupk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gaodtocad.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gnwokhcmg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjtziikni.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gjhbmcaff.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gnfptgdmt.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gllwccpqe.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtnoczzor.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gaybaygwf.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gtyrheaty.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/giavmuxde.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/goavhdevc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gksyjzyto.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gljjhxpkl.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gbxmfmurk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gcllifbjb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpqvbusdg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/galbfedob.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggdthtmal.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggfmbimyg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbihpxulm.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gvrbmedzq.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gnhdienfs.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gmogekiqe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsxlvtezv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwjcdqnmd.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzgsdryuq.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gofficsfl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/guzkcbqbh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gmcapojkg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghhvvvnvi.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gzqtdvmfj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gmvuzpanb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gicancime.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkfjsklvr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcqvmkvei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyjrewjpg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gkqalmsmv.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/guonlqtdp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/grktwrxud.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtbsexivb.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gyrimgzea.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/giftpcgvk.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ginwuadmo.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gcfvusgqz.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsiawwecd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gymjbitiv.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gvdlxluwv.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gavbulxia.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gfhorowvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/giphzrsnk.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gdcjunsrp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gzdnibvin.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ganxperxl.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/garttxffi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gefibfpdb.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gtlwxqwpn.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gnuxpkazd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/guskvywoy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gwpvsvzts.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gldnzslxq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gthhgdhmk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvnjoxaxo.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gzhtqxnnq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gpardhppx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gpdxmalpa.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gbprtqzpc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gfmusiwrd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkiujebar.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gfliirmxn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gqhwqjrns.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gvgjhscyb.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gdjwhtlqv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ggyhzrlwa.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gzqqwvgig.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gojzvtyul.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/ghisaaspl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/grwfgtktv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjqdtvcaa.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gultyxawj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gyziaxcjp.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/genfsltew.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gltljafcm.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gkxosroqf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gnosveyeu.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxrpjfwcw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gafobxpjw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gtdyixfvb.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghduvxkvn.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjldhqrjr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzlvbnnpt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnoeeiauq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gzvpipols.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gydvpllqn.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gfeojeuoz.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/geindnfen.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gddkdedpm.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbjxhgabk.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gwpenqkph.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpwrzjzrj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gegssjfas.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gbqapwxzr.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gvpdoqvuu.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/genywijpe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gcevxxigd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gddnbvwqm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gxkikinpv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gnyaoqloq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/guaknvrfv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gcmoyrhaj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gckzlbdra.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gavjfmspw.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gfkescmsq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gzhdxymql.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gxcqugzio.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gdmezhxrc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/guisgmetb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gldrsawno.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gqacqbojd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gkbmubawg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gvaeoohre.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gdvecqdlx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gspentvel.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gepfgsgpw.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gawiuxlfv.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/giggemwbr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gmshpfhbc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gcabmeisv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/glfsjvjkn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gklasdouv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gopbagqtu.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gxydsuyfw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grnvbkzvc.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gnkkgmvni.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gjjnalate.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gllynflsy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpusbaqph.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gajkuhejc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gbtoezwzw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gnedlgusx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/glnbgxwmj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gmxyngrlo.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gsjkytlox.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gussrucwg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/geeetvtve.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqflhbhkk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gkywdghlc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfltchxjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gtcvsfgwy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gxacvtuoq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gpebpyxhc.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/giknktfab.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gyabrjtep.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbuotwtzz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/guvshyfhd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvsvbnsrm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyxdaloym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/ghcuyenrh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gmloxtcqk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gigskbjsq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gaslyxufd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gqnvjmgxz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gfwlioumv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gxtxoogxs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpaxxquce.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glkuposzx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gwufapgwc.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gshhahyci.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqctqpmdx.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gthwfzfnx.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gkjpbfimv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gkbsyrxvh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gapygmfhi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gsmkkrzct.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gljmnmfve.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/guxrhaluu.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gwpqgbvxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gzqplqbxx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gwpnetqfh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gnmvukwya.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gfiwkghqr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gooiuaqjj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/glxmsvxdn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/giwxoemkv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/ghbbgbzgg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/giwwszvhv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/giqdrdfqp.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gicvjtybe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gxgqgkigi.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/grhkbkkeg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gaxnsdsvg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxqxkomxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gvrvvmpvg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gjkxlyjlu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gtcpnsbft.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gyzjrvirt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gzhpbpwxp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gazreeclf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gbeebnlwg.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gswtmipnj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gwnatqkpm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gzymnzhzj.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gwxdbtbul.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gbxcqgbwj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gdvuugsib.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gqggvquod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gbbissqrr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/givwaecqe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gbdlcvcil.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gyqswxrmc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/glpqiimpf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gtepbsfuc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gcnpmqyrz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gwsaqumcj.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gyitdrxnf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gobyaoqhf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gjrispspu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gtzvhdgva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gfqqljnho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gpjzkczmm.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gnhvrutzj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gquldrfvc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpljnojsv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goxnzankk.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gpgngosaf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdqvkpbvo.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gywkmtmcz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gzwfqgyss.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzsmxsbuy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gqdkcgcpb.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gmtjscgcu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gsdqoeaiw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gvyzgvrox.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/geuxuwsim.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gthalokjp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gleapzzam.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gyiwjzilk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gfttjhnag.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gfwmpbbkd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gbhqefsqh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gltiwzcop.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gtcarumtz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ghmnofaek.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gvgqrwmoz.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gpmkxptxb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gyhsoycmt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gsdxnotbx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gdhnuwkjl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gulzfnldi.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gloglactd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gxeyfuqff.sHtML


<!-- 参考信息 -->