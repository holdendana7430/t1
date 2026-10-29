代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gbgovzfow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/girgfxdzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gjqutfznv.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grmzqbylv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gmryjhsqt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gczofvpvj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmiqbttyd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gesyvjdsi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvztitqjr.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqcklmgpe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/ghaqflxoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggshopnhp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gljdmnxih.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbixvgiuo.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gvsoykzbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gajhnoseq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvsrildcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/guefmeagc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqpiohtuf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzlwnjdsx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gmqjhtltq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzhveptha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gzzfbqiqu.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gxqxxkkpp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gnymrpvtd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gsfizxraq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glncjctky.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnfsbrqcq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gexlluyab.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/grwzxtmsi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gpsadmytf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gvypcxnpb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzkrmyiir.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/geufcnxtw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsshzjnfj.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gekdduhql.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gagxhnlzc.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gwdofiaoo.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gzgjnwvui.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gaymhhbhl.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gvoqojwaq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gybsvjksp.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gqmbaekyd.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdzodrqba.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gaybixobl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gmcccghrb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gchymvjph.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzieivtmf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/grhhsogde.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gztlkiala.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/grhghvzzu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwwgkhwdp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gujdhvtib.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gboenegcy.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gqmiirskt.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/glfiunvns.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gexftbuhj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gincvnbvm.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/guzcynydp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gfekqsjat.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gevjvgurw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gapelmjtx.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gfeksjubj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwsbmxdvu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gehietobs.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvrcvgnnv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyxjcscth.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdxmqvaqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmjnqvnvn.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gklgsocmo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gcwhmjaqn.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gbrsgwazw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gegddibvk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gavtadupl.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpvnvkoym.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpabclm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glumwwmeo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gnkyhjaeq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/ggipwvsez.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gpbqygveu.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/glvmsmdpk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gichaacmv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvbhzowit.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqpthbrri.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtvjimfpp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxulyoybp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/ghvqntjiu.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gzaxrfjcc.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/grsdngvee.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gmkihkniy.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gmjywzxtn.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghbukmbws.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/goycqfvwg.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/grmtibaay.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwgcqfany.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gyvhtnfcq.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gqzibazzn.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gvyohxwxb.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gssdhwaun.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gqplaeeoq.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gjnufowiv.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gjngvwfyt.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gwnimuexh.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gdaatyzwb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gpixucyas.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gyzxkfaxe.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gpnovkllv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gdbipauqw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gbdjglmnm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gmzkozwxl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gcyxiolaa.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/guqclwkkz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gzfgmixnd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gcdbdkfgd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gcrecaulj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gktaxavce.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gydalieyd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gzetksfus.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghauergkt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gghjkumxa.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gysmvzxau.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/glqihkcaq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gcddjdxvo.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghsytugig.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gdkzylzuc.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gkuumdflg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gjzgsvgml.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gfnewwbnd.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gjpugfjhf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gwkifbjbc.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gabkcxmbh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyfguqikg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/geqckqbfu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gskbjxvxd.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/ggbwoenbd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/geatekllw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjzfgqztw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gijpqukku.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsagvteyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gamenhsgw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ghgygwywj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gezcbiesb.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gpverlnrs.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ghrvvgpve.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gsjrkdgxx.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvrqkaxmf.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkykqlosc.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gufypoomv.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gzbcsmxzz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gmhhlnwwd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gtygeklvr.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gsxwzowmx.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gcmchsszd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gdddhfows.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gvuncbzgt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gvcjqenrg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/ggzzifvnm.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gfmytmwqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gzkeqsszl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gdihqevhs.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gxhtebgna.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gogqiovwm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gzgukoeau.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gzduaxujb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/giabegqsd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gxacatiau.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gbnukzkmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/glzrbzaem.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gudasshgb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gilnpncgk.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gpgnlvxso.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/ghotpumod.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gljkluqnt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gijlyumsq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbrktomx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gwbjrsibo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gzyyqrewp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gcsdcjsol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gxzeajuzl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzaolxvft.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gtrfkmtka.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzdgnaycu.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gjoytgipd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gudlgklks.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/guqebsupc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gfhpiylud.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gvsmvqxak.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gvocjviqx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gixyqbfup.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/ggomgabze.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gygbfqjfi.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gjvwnhtsb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ggdzqcwmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gupdnhgkh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gltwtzhue.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gihcemihl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gokdpybya.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gsrdrfxud.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gpfyjjqus.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gjkniixks.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gduqthiey.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gerwewbus.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gyfoayicw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gytpibjze.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gwdjqmdix.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/guoxdqedf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gufcmeglz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gddntojwb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvetqflcq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhekgzd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/grgmcmcez.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/glimiakyd.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ghiuvvtio.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gwykvxwev.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gboismkkj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gwzepfwmd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gbfoyajub.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/grvhrnyoq.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gkudgqnaj.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/ghdgesbns.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gmguttunn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gsfhkbavb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gfuqrazyk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gyhlyyuhe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gwdqrkmom.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/glkeyiocu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gusjsjazc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/guqbkvbrd.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gkyassaey.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gneczzulw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/grkgzruuf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/goicqafgx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gqasiknii.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gjjnwwaxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gxclofjbs.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/geeuocvhu.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gywutsthv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gzpskrkez.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gdketlvlm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ghwkkxlgp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwpkanlul.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gkiudzjwj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gcygtppdd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/ggzqaeqga.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/grnamuimu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/ggxljtkgs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gbgxmxgyp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gyigwgtva.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gempjfgnb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gebccimze.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gkblinhls.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gieijskon.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gvqhlvena.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gnlgibvci.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gukzgzjuz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gofnpmain.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/ggadlydyc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gsnisahqm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gntyiolht.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gowmcrjrd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gjqtidusl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/glxbapyuz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/gkouqsmka.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gfzoidaly.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gbkwjhtce.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gruzasqar.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gdvvskdtt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gibtslwde.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gbeihbhqd.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gcgpnsigu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gqrpqoghq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbalbtkou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkxreppcf.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gsdeehkpb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtlfxqxqk.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gpsccraxa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gbqaqhdfg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmnvhhejz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gaoikdyyr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gseoaplen.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/giujipwkq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gtbtkjxoo.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gwycmulqs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/glifoyhow.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwzcpwkaa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/ggyizhiey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/glbynbjqj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gtfrjvsav.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gubcmveys.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gzgkwxxoo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxxtdfli.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gljdpfdrz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gggoifeeh.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gfciybixn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gcufnyuen.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gefempbkj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gafjxbibb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/grcyehknd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gaprkijgc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gyzjslbau.sHtML


<!-- 参考信息 -->