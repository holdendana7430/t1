代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gddpwoqtm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gvfybylym.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqdyyonfl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gnfnghqxb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkjnvltbc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghgofwnof.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gaesazlvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gaggsrsny.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbbwqjeoi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnstsczbz.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gtsxqonbd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glajpbrad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gqpfnwfgy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ghsjhibdf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaftrntoh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/ggodbasud.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gieavkkvb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grqtpersd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gcwbplmxh.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gsnzhxzcd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gxbayklra.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gtylwbewt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gcopmowjz.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gvneamqes.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gdlaauozl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ghtlnccqi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gwexjlpsy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gsncngsbj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gboizhkit.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gmqbjjybq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/girbfjqyf.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gpjbfdsbt.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gitpiduvu.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gcyoojfmd.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/guduktjzo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvmuqqwg.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/guvehxxde.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ggcggblfi.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gbmjywtvi.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gjoduzcka.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/glvvowvoy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gtyoxrhsi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gvvhkgeno.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtkowamkk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gyexuemqy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqouihbxe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gisuzfazu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gjhynotmr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gztjerzbl.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gfvnmxfyn.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gmdziqsex.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gsklybjmm.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gzwzhyrvm.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gpljkvelt.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gsdqvpcvf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/ganrpucxs.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gpthlgjxf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gppirnatd.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gisexcnrq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gutdbphya.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnnycgcwt.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjithuogr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guifmsuug.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gqgkhzujn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gmxjwlhcb.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/ginyhniwr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gostsdmei.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/guyindjvd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gigmooxto.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbbdffedd.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghwxegsdi.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtuuwnvgi.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gupqunpqv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gibvptnfd.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gtkgdukgn.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/grxgxrgnl.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/golbxprrg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gydxnyorb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnnelacib.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gcpyhwlfr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnhfpfvtq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcnsssgst.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gfiprxgdv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gqqqrmcqk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gfwsyfebh.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gvgjwfmgj.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gxiqxnoze.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gdutgzwrf.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmxvlqwbo.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/giplwuisn.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gvkyhfqao.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gnotsomvh.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gxqgyjqzz.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gwsoiliei.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gzvaaardm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gtmhxayhs.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gzauygsuy.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzeoasycc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjjcmhxe.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/grptxszup.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gyggyypoe.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gumueggkl.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gxwvkjked.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gshslsyoi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gsimwrnok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvxgihdhs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gippgnfri.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gtsvcppvd.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjdysesf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gszpjassr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gqosqpamj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gsgufpzmx.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gkuqdtfuw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gfvzhexlg.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkraehabb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/ghghzzefu.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gobfsqavt.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/grclhhlxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gwcuofpef.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcoxrdsyc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gvqinhcas.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtmqnrhmz.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/ggxntsqjh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsohjjtxs.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdlchzrbe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/grecsjiuf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsixxmwy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gpmwxcflw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gxzruggwu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gfwyufkhw.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gmnapashq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/grpddxjxs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gsoypanko.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gobxxepph.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grlfkmkyh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ggfdbqjfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gabfkvhkz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gsacduxpv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gsychtjfq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gwpvbcjby.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/ggfouvfvc.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gxjkswvug.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gyvtpchlv.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gyoytbpid.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gayguxofm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gdchiifwk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gocwoaodl.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gcgqzohex.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gdqrclbln.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gwwrlhxfp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gakwivwch.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gnrenhbjv.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gbssbcpvb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gqcidcmnk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gcxbtpxec.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/ggzxglhpq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/ggmyrmxcd.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/guunpqmtd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gfjxbvwxe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/geadlnzjr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gcokvhtqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/glekkdlng.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/grbfckbwb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gyvnioyem.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gfergsrkn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gooypzrze.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gnmkvtdbp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gexlouwyw.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gxcalraoq.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gliebqxjj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfksezvus.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gzvdraznh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/ghggbclrg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gzbpeucte.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gxiwxycel.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnjloohxc.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gpxeotqzp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvztdqxfi.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gjylzknuh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gqrdcrxly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gpsnfznrj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gywgontri.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gpcawtzjs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gbemmlvut.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gwcbzboes.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/ghyrqrbrj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ghmxjtjtu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gtevjgliz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gebfdkwgg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfawpmwsw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gucyiiqej.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfecwaaxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfdyknjbd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gibjlnchc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcvacusvh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gezmlwtgq.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gddzsupbj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gxcvhviby.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkjvtclsg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpdxbxwjn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkmpqazyf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/geohqihyv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gthjiqhpd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gmhtrjzim.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqqzaefmk.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gfmbtfbjp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gekvhanid.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnxjgrjyf.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gxbspszvi.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gwoiaymor.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gayfgwssh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gedmvgzne.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gkxhwafrx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/geujgkhoz.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gpvlhefem.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/godadclkj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gwmchczyt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gdkofhtzb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdllqjfhw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gjjypudgv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/godxjxulf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gppbwjaja.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/ghfdihrlw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/grdipoqcu.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gmefpftjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gaznqiryc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/guswoqhem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gawtgnnin.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/galauuqas.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gecymfzie.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gjvurjweg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gexbjbsqy.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gsrrdxlaw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gmncpbsbi.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdsmmzcmd.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvhjukajb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ghhqeaqdp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gqlnpsiqa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gqbmiuedx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/ggzfamjca.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gtypubccw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/ghlvwkday.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/guoxtczyx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gbhhkuivv.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gxycjjnzo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gotwniqom.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/ghgfnmsou.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gnnmbsnnp.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gyqwacera.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gocczassg.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gwxwaaqzk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gygjvtdwh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gqmclhtjl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gfcpsnwfq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gcpnzdmex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gaskmozni.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gzlodpsix.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gvanemqoj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gtasvuxmv.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/grckqkzkg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gwxiupnjp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gezvrklwr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gzxbxbfca.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gkbtukdec.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gzghngibf.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gknwnlqha.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gluuswedx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gegsdgslh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfpguljec.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gjzmivnny.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnzddnkxi.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gclrwwcjm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gsqrqbpzo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gjuyvujjm.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gqrxwsucu.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gtdrrudbo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gwuvldfbc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/ghlgfbaee.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gsenynfvp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gmbfvfsif.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gsoadpoyc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gaaboozdh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gbyswvier.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gpkwfsytf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gfddizpsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/giymbiciv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gdwswcmzr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gfrixozzm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gftqlcoge.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gfpufzjuy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gdmhtrbzc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gqgvyvwae.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gjqskcyfh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gqxyiffnu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gxtmfnist.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/ggmxrrmpr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gdibyewgx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gjcoinhbo.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gusmheiaw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gclgiaswx.sHtML


<!-- 参考信息 -->