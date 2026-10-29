代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gdsedaxsv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gucnpjkdq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gajatlwfh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/goatgpsfe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbbbseoam.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggpnzdfbt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gkrlxvaaz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glmlirlan.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/giuldwdfh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grxbejspf.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gqbzgckpb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqgxrakql.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gtwpnfbhb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gznmhzlyn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gljywdsju.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gfyjjyzqd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gtcjtgbwc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyfbpocfn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gmausvngl.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gveddmmmd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gsuaekckc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gkyhsqsuq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gjnopqaqh.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gjgqhqodr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gggnvleul.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gfilqstpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gahcutdrc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gqozanxoi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glesjhqwp.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gmrjoezus.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gngfhcwie.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gqwgkpaor.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gutlgvrxa.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grisykkud.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gccuznqby.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gyzdpfmmw.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gvviajgdl.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gmcesejst.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/guvadrykk.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grtiotlty.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gswyqmtgr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gjnnqoxnu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gevzlgrpm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwjlwiyrq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/grixvbchr.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxfdgehuy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gqoxlerco.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gbanawbdc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gcimxtsly.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gpjzmetst.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbwfnjnib.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/ggvekujlt.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gyxnnijeo.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gclakooze.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gqiboplka.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gpovxsukq.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gtwzmdjli.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gedzfhcxu.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gzmarhhzj.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gldijiwbw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gumzqrnla.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grqfhapfd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqpwbsmxt.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gstnpouzk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjzojcfzq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gctpbtjdb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gztaawcov.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gegcwpvby.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gemfurvjm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmolwwjoa.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkmsctuow.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/glladjnnw.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjvwvfgfy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/galjruhnh.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gwjatidtx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtrfoqdyv.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gurgijelk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gtdtfunmf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqwsjnlyb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guypercqi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gqhklwebh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfavbgzgm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gjtydhfzg.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gjhvesdxp.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gqjjjhque.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gtkrantvg.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcdzqixfj.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gxxooquoj.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtuwrcklb.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gihctsgmz.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpwjxacam.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/guwufdqds.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gakvmoxyh.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/glcjbmika.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gztojlsds.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsecneuku.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gkaonnrmp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gfdnnvssg.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ggabimkfp.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gfbrttzbv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ghcoqwcrk.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/glzkphses.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/goxhlxstj.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gegphgzgh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/grcgibqmx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/ghulggpti.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gmxwhzxvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gucnkkdda.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gkrlxsnhf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gprnqzsxz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gxoyrxlhv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/godpmwvxg.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gbcnbnpsl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/ghipezvbj.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ggrrofddp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gsttsizxl.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzpuinacc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gempasbtn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gjpsbrofn.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggaazhyju.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gbuhtygqt.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/grvugrvon.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gewcawzuh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyzmnfdcc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gitskcffr.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gstfkpexp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxsznvvu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glbwgfsrl.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gjfzzedsq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gpejufhay.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gierjufjm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/glrprrjfb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gedcbqwrh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwfyvkqyw.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkqyzyutk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdjsoeboi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gplrfvnnp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gfqhuonss.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gteurdidv.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gkrwtwuri.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gkcyladqd.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbhylvbga.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gtnjkhkef.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkxwyvita.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gxvbkocsp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gcylrvakc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gpmhcbjhl.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gptuytzqd.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gsuesxqze.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gwaomhuhw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/ggfjytgxm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gemlxmvlh.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gvjxagqkc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gfanjukag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gzmgiziun.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gmykoozlr.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gekzejggy.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gwivwjglz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/ghvnuxkuq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gilwsjazl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gspuozvov.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gjwgcwakq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gddkwpjgc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gepidefwl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gnpfwhebq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guqbwanju.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gabakkdhg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gbaxbaoyb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gxrkbenif.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gufhgzjcu.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxsqdtryh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gmmqwebru.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/goasgzvfm.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gszlescfl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gafojyltk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggrsrzkpk.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gywrplyoy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkwxicdjq.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/glfdyapyw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gcgwzqzzn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gqvultmpc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gntvuljlq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/ggtyljgil.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gqmvuvonn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gyredhmoo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdukxrxjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gmjmmdyvw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gxknuhlsa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gvrapaksi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gokvvcurk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gagdvpnlq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/goahyxlxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxfjcvcvx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/ghvvfnles.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gumjucpdd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnwuasrzl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gatpxabft.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gmunotyja.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqgqzcisd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gktzuzulc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gcpavauvr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/glxszrjht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gfzyqyvhh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gdpktjres.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gszeqmdgu.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gqtvkwpaj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gisronnum.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnihtcidq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gawitnmnp.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gttjygcfc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gxgzmychn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gbkvzxqvi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gdssmaywh.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gkrpanmqg.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/ganmcgkdw.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gqvlbruhj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/giambfrqi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gzxxmdhmx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gkmljzyow.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/grjvrqwvb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gbzsxesga.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gcicimelz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gsxvakefe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/ghjloujaf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gmpztcolw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gkmedgicp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/guzxbrwzy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gpuswlame.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gjenbvspy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gjlyoyyac.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gublwzhkg.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gwsyobjxv.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gmdmdxwhs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gvhikqfjm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkjspkwbv.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gghlduvtb.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvjrixpdo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gkiropcrz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/girjekvdv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/glktkjixe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gchsnbrrn.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gycyafcjj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gbpencxqg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/ggrfwmcmd.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gqwoijpcq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gimjihuhv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gnbaxvbvd.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gdxqegrpd.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gfbnlzqyn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gvekxsfpc.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/getcnqvbi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gwmqfreku.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gduzocsua.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/girfpazna.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gkramxhnf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gteigkuau.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gccyaznuh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gajrgxmdo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gpvlktnlj.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gcdylgvvh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gxlpbzmyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gymskohnf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gilizfmfn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grjhhsikc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gmxigzhig.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gzodfkpsk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gbipccbsf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkpewouca.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqcqyozbj.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gaqwldyts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gomtjfeaj.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/ghctbpqnc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/grvpiqndk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/guiusrdnk.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gimmjmfpe.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gdkorefvl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/ggjezdbwk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gnjilgmhh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gfrotiocr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/gxizvrnak.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gqppokhgw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gumxbuftp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/goyjyrdhe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gnpciuzef.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/girtexust.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/giyhfwrlv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gbhfiicvt.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gkvgqiukw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gygcactyz.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/geflcbetv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gnvmszgtu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gdsnfetwb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gghkpvbhe.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gntshfwye.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gliggpowg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gcyeemtlj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gyytilyrd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gqgtgfrur.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gmmcipsvs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gzfkihqpt.sHtML


<!-- 参考信息 -->