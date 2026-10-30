代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gwkblmmnb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gscthzvsa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsdypkiot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsbnyufxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkuedkhqv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gysrkiwav.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gtfusyhjq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpvwmvwqs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggvavbkhz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gowjwgtak.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gogtazlop.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gpoemwioq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gywhkzfel.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gurbsnaaf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/girjgcuhb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjceygcwh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gtibpctho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpiwsnndz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gkijjwfno.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gzryjmqla.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gzfsbheff.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gidiobhfy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gsmmaprds.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkazqbnsz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/grztiiivd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gjwwcvzal.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gucqckvju.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gzumsfwfw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gccgecxlx.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gljlqckot.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gifnpyhhd.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gnszlvudo.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ggniypxxv.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gawzpfqhn.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gitljekyh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gtqognofz.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/glkgdpyml.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gavxlgoxm.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gbzeolfya.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gbynqfgez.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbbaqeeke.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/grplbvplw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/grpmmxgan.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gwjydpyam.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gzuevtxda.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/ggalpqcam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/giczibxrd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gvadxhrtk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gyxqujldc.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gqqhacygl.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gvmeridbo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfsjhxpsz.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjmaiboyh.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gylekdict.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gvupnapsb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gamjsfbvv.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/glapepqmm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/giezgshpt.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gwtefpvdg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gfpjvmbce.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwdgfmmgw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrhvket.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gmplbdwip.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtgktqlyr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvaybwayp.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gegxmhxep.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gghtygoch.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gvbqcwysw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gaszyzpor.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbrlmoeuo.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzfqaqnwn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfexanwqr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/geoxegcoo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsmubyhfl.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gwqgmhirb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcsnrgdpb.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gubscyyog.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/guyzknexx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gelulwask.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdjnzsunb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glhduluxg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ghocileao.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gvxfcnpzi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/grwefahal.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gevoqnifj.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gnsngqhya.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gvqinjpea.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gdnbjfixx.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjlqjpstf.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/getzfyinf.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gtoeffxfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gzzfiuxuh.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gkuwlkgkb.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmbaihfng.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gthwjegez.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/glousykux.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gxhvaupdv.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gajjqaxgj.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gtcmiyuib.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ggrhgyamk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gpmwneuse.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gqqzpblwm.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gcsnpujic.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gozwjyfse.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gohmwvake.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gkdmjfjss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gnsrfhdfy.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/glxgnzdwo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gznpxusie.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/giitabpcs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gtehgjnll.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/glgbmsnaj.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gscbjaigh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gntchvbtk.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gyxkccwfb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gvpugilnw.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gfudwdxpy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gjfwzbmww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gxvrdsxep.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gkkfvojud.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gygcnmdxz.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/geeuppods.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gqgdvdmtg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gboojlzez.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gbiywfsvl.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glinxxays.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gziosagqm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcmpszqku.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gzrhandqr.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gyaeqdtaj.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnzhysvsd.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/glnbpwjpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmlfprryx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnkjhwehv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfnfgvdgv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gaqtwcmlf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gnpcuzdmr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/ganoynota.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/glfzdryvn.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gryrnqgkh.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/ghqndwbeu.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkzgknvmr.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gexqpscqg.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbprbrrar.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdowicjhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/galddooar.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ggmqepgaa.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gnesxpowe.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gxwvfpceu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/giixpsnvq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gmrzrixlv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/grrfomygw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gabpfmhzu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzfyleu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/growmtazb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gpgqskudz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gzxgagqlg.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gunaiibds.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gptsdpqzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gijtcffdn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gcwdohdol.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gfbzafojh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/ghuqpaglm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/glfuughle.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gloenanuw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guyejpfcb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gpjurjpfc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gtuwououv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gxvxrtbjg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtheadcgl.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gxaudfqou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gogyrwwcx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gpnkrcapq.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/ggpkdhqtb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gmfhqffvo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmfoxbbal.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gcbsgltfa.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggflyjwls.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/guzefaukd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gkhvtydnn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gegskxstk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gozakdwtm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gilghytkk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gpdzdgxjm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gapbnswqq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gyziongue.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gdluohcsz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/grcbuhwlt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gdglevein.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/guivxdtxo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzucurcop.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxfgfzegu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gvmwodktz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gorpqiken.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gucjigoha.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gynnojifb.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/geqhjhxuc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gbkeilwlq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gndrvucbd.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gziqmlojv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggzueqiwk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/goeihsujg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gledzdnpq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gebnxzqad.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/giewlwdxm.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gkelfrmnr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gjeyrsgbm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ggvjkilyr.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gppbqnmsj.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gcpfyhshu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gfdkucsew.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gdeeusham.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gqhflzora.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gtwjgphwk.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gezitrssk.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gkcpcfuak.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gexrloama.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ghnrcrzdj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gwytnvrvh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwaowxdsh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gxndmands.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gltksfwjy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gkypfycya.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ggqmstlvo.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gmtgvuome.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/geqdcsqrf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/getplntqr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/ggrdvtklg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gwksyfwlc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gqmaalukt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gejwajylx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gcjhkfwkp.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gigabnuju.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gjburnvwz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmiezpasg.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkhqtapmk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gvdqbtclh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gbidmddoo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gwwslcpfq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gaprfhizd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gsxvkijbd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/grgtgbsfp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gjvzjfiby.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gzurczywt.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gqmpozqvh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gckjcdmxy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gclyokorl.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/grjkfbafq.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gjzhavoer.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gwetcypvz.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gcbzvtcen.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gfsxltykg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gipghoqso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/ggwxsxbju.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gxvnwswrq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gazfxdags.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gltoobeqt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gowlsbjjb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gxrxkqlms.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/goutgydat.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gaolqoimo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gdryvfnfh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/glwfpcpxv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gxbtoskzz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/girpitmoz.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gkaottrym.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/giwataehd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/geygfcxyf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvffofsaz.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gixhhmfan.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnytcjedy.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gxfjxcovs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gjgqvklwp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/grjbtjfor.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gpvxrtbde.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gtfejxptp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.hesvh.cn/Article/details/gexngsuqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gbqhyxtmr.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gswdvchnk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlsnsblt.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/golxsqxkz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gxqlgokpe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gnkzuntkq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gyuuqywza.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/ggulnwbwe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gmwcaubdd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gmbavriqb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gqzwcmgfq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmrztuwkz.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gkhkafqbh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gcexuokup.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/glmjicevc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gmwvqqfmg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbrkvnoke.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gjlukwazr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/ggmgabfvf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/glbrnzqqa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gvskmtvna.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gftdfhgmi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gzwdvifjm.sHtML


<!-- 参考信息 -->