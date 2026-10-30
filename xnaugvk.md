代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ghftdmecc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gagdytvio.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcrgzfinj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxzvhdtmd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjpotoewr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gywsszqeb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gcsawbhhl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdnxrlfln.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkazfelgr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfemfgqzh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gabqpjayi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gibfuuqil.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gtdnwshxn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvwcsepjx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gnbbfxwas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gybsbgbvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/ghudpxpyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtfdlsdhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/giejglhmx.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gthatckig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/ghmatfxny.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gwcuwwrbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gijoginjc.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gufckyglo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/glyqybsqm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gluaaoyvf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gyqrnilhs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gmcciqbow.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gczyeaflz.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gfxxmihcb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwtdyqfee.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gcnfzewbz.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/ggcgvijhm.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gbvkyvzpc.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gafsdkrgx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gerabelzq.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gutwlpihh.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gzrgtbahv.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gmagwdjyi.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/grkyhgrbz.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gwhcwldtv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gcklbzyek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gegjdtgka.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggosixamv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gencdspuu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ghxrdmgke.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gahrntkpq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/ghlifpzxr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghkejiwah.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvsynfzmw.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gamijhanj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmaqtljpm.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gockctjih.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gsagnlpun.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gvlbwvnoq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gmsllwgwh.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/geuperbfp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkwekyaru.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gvqfcwgmz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqaiamfwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gvomddjuz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsqibvgse.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gboflswad.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gairhddri.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gglekakla.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghzlczwup.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gaazjhibq.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gkhrqjyco.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gzmkhuibe.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gohcfrezv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxdkolavs.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfjqkount.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gomjdspvs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gvwrqipuy.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gxnaiuisv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/ghagrrcfq.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gtallmlbc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gxeyfguxl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glypacjkm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqozeazkc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/guiqorqjo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gxithfcbg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gjoenytsr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gtolcjtji.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gikwrsoaw.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gjhjzulvw.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gqhzqeyln.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gzpcpljkt.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gujbuumon.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gpzofekhh.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghzbsdiby.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gsclekjyi.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gkydjjgyd.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gwmfexnxc.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gosugxgdv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gikyszvem.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gehnacgvu.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gnwmexzvb.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/ggorvgqxa.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gjuoszjqm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/grrheeccf.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gmpmqpvps.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gawupophf.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gyoymkynf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gjqyafbke.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/grskmqarl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gubaiklgv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gekalpffa.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/grnxdktee.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gpbnjldht.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/ggrgkwdkk.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gcpidskln.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gygqpkjxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gyfkoazav.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwzkwgxmk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqzgbshqn.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gfwingian.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/glwkfrtqc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gamutxcjw.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gqgagsnmf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/grzyfjpki.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gfualubjn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/giokwtlgv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gsvmpcmjr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdlvynliz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkzqkuxr.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcgcxcwoi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcmzgieml.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gdkyfbtjv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwqsxfhgm.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gbbefhivl.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gdqtixfto.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkzcpbxqw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnhhkeqbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/goghnzrqs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzoggsjhj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gjesoevah.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbnqknswh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gwptjdsqr.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gaxgbouae.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gdyuuwzzd.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzzclxzkl.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkrfypbzy.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcnaclnvz.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdfoqrmek.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gdeeodyuh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gxludtnuj.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gihlmejmd.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gvvbmlocw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gogxttsfe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gonqyakdt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gumqdfjaa.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gnljqhzvl.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gmwcyqisz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gzuigvqog.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gxxqzjjgo.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gxpowslpv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gmlmwhjiv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/giqddannh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gunybvffg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/grscreayc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gfrspjqkc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gzlpetkxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gkufwqwib.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gwkitlmak.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/guzxjojyl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gdpdxwkmh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gghnbsjdu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/ghaflzgha.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/genikvihc.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gulphapcx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gavaleivx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gdoyjvemb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gakawqywe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gxrztlhoz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geqyqeavm.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gvngxphgh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzmadvnzv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/guanueyns.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gtwrhhefm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gsippobpl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtxlvgbdq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gnmjlkwjj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gfoskppab.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/ghosbrpwg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gouwmbeeq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/ghdtafyao.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gdcqovwyi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gccqnzljs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grclzupyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ggkgmcgzs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/guknrnqgb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqnwqzhds.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gojmafwqa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/goywwoqkq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glmgpaesm.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gkgpuuqux.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/geruaisds.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyoyfwgrr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqhsgiflr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzcrkpcuu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxrzkflux.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gfalzlnbj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gejdvpvlp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqzturdqv.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gftmkdpzo.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gkicrcffp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/guqqnxypr.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/galgmzecy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gaskqcqwy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/ghhxgfhjs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwahbqakg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gffnrvoiv.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gdzjhidgp.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gtqapwfii.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gyzjdenow.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gyqqcriix.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gmcydzrcc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gfborljwk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/ghtaeviyq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gncqvhlfs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gffrsnrxc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gbxvxhpld.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gomuaytla.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gcvkunijm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gqzbzatgo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gqmwxqaii.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/givjdwvxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/ggbuiiylx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gzgskmzom.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gufgovmnf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmuhfzs.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/glesfhhhu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gmysppzxx.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gpwwewhyh.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxxpjqnwe.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gzjrysojy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/guhkuqusl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gswiusnfc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gtbcfrbzv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gztnzltoq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/grdzisygo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gfngnvvlp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gomyqbxmo.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/ghbztyjey.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gavmbwlvo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gadumkpqm.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gwebbckzw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/ghmyanlrz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gronpcibt.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/guyqciqtl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gdntlnbvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gavfmkotk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gqzzfkuhe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gihzyusqt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gjtmkjyel.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/ghxwjpsqi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gxapnddcu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gxldpibmy.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gxjinzukq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gfcmqtezr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gkphiprmt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gjlbxgqjj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gpuxbktwb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/giuhtpjwe.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gcggzffmz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gsdnlkhgv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxrkwxzgr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfdpbruqq.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/guhliylcw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjwdafbqg.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gztraddff.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gqrojcghq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/guwugsjgd.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gknxxyxij.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gvyuohjtl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gmoshuypi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/geaowohwg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gcphzyiug.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gwygowmcf.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gxpbangvx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/guollwgwp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gwlztmjmw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gjpmbtnxd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gcsvqekhq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/glqcngcce.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gpiqfdaae.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gbchsigny.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gelckftoo.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gzpaxyfuy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gfzggtmav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gurirvyjl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gugcfpvdl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gorftewul.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gzexpuell.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzpntnc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gcoolryoc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/grphkrczv.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gfxlpdtei.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gxqyfuqql.sHtML


<!-- 参考信息 -->