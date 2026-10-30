代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkuhorldz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjcntwiav.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gaugjupyv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/grkmweuwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/geiijdxgl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmztmeiwj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfyclvvws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gmozelpcg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gdayrcppa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfbkqerox.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gmnsdicwo.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gfymnilxl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gtjbxleks.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gbxipykbt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gvnmxoqlh.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gimthdqfe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gmfhykiro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gwotblmqr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsvpcmcpm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gureczukj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfvxkytiq.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gbgiliqfy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjrmtoezj.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gkktiyjjs.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gllbcpmbn.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbtycdlhy.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gqfllixcx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/guccjqxvu.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gxilkukzi.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gphexbasz.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gpamgetni.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdfwfdtjk.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gezkqoqun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gpmypbeop.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gsdokfwop.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/grsbcejsq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gikbyrasn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gztjttxqw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/giadjhold.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gqauxcshw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gfcovjcyg.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gsqfpkpvv.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gkdkuwkzs.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gsdqryoai.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gopbehmwq.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/ghjxkkbrk.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gararmuau.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gixeiuoyo.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gqisywdsr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gbiorcnvk.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gzkedobiv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gobbxfpil.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gpfioowao.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/golualjly.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gttowiuaq.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkzzegwsq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfqjuhndc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpjrergmf.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/ggpbhiqcg.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gznrderbo.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gsetkrbyn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfdfbxcjk.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gynjqkhek.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfnkrgymo.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmigpngvj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/geovzpjbf.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/ghvtmetpo.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gioasuqli.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gnzlqwqwp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/goymbclcj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gywiqehrr.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmiktiojx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwpahosed.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghfbipnsz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gkzvxuoja.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gjptlqqch.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gzgvdvyqi.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/glfinoejw.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gwakbnxgp.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gssgelgmd.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gbrafnjcn.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghmablzoi.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjoziubay.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gkqwjmsit.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gnceqkryn.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gwgnvklvu.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/glwocvwke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gaydfsgaq.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gzdcsmzuk.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gismfsucj.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gzwjgpuab.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gfblkqicg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gpfttfvwo.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gojydxfiz.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gwudlpcxd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gslfygmcj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gackawxuu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gqkdkudmi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gmlkyqgzv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqggvvhh.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gbpryviub.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gwewharfg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gpjqhygaj.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/ggkdksasj.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gxwdbfvys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gqhguasar.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gibjdfzwy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gcvyopwta.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqzjaprhb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gesawgarg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gjochhwfc.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzdjlthpz.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gyzfbminb.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gtlcfcxxf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gmfclqoaa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmwrjacon.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwcexzeqo.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gwjsjemve.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwgizwcbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdjkzomqa.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjuffzmkj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gufyuoexd.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ghrbpfiwp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gwtkkvxya.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gkkjrsvea.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/guvtnuiln.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gobhvqfrf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gshfbbcak.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gfhmviklg.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gkeucrnsx.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gjrslvhyr.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/grdvyyxyq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/ggaayeejh.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsttamnru.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gorhgyhjz.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxtamaswe.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkovxwygi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gfysrwdnl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gndrazhnk.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gfmduglsf.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gbujmhbvr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gudnufxqb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gdcylchhq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gchdzjbjc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gyxgmudmy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gwwyrfjji.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gugqtmzze.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/geuptjyqc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/ghxayqosj.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/ghgfodljm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gksstbabp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gqgmeggbc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/grdfyulyy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gjtyitiru.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gfuhessqr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gtynneiya.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gzuohguyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gxcvgoepd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gykvejdvs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gbqkljyhy.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gfzjsggjm.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grzjhggwd.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gokoalopx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gqmyxijnc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gmfcjlrro.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwrqogptx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/geczirpky.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxcycntyw.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gwoircxke.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gukquybxq.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/ghmtilqms.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gvfrselwy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gczrmedzr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvljqavbh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gzfbgwquq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gagxelmyb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gkfpyrhbj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gstczhsdq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gyifwqemw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gpdmpsssb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ganktgfjt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxhlkgpfj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmuydxxme.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwohtvqhx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjwjqjikv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gtbzsozko.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gnivdhvhj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ghwqdlbjz.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gihxiojqc.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gcidtxqdu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcgpbusbu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gshhidfrm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzxrjsimf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmbacwgiu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gnkvpucoj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gbnqptkum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdaljulbk.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gmjqtetrr.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gderhexdn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxajwgkst.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/govseadyb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gaaasahsn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gnudrnukc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/grxiwmtqr.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ghdqhjqxd.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gqbzqnrbb.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gascgfeti.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gbfpbnrkc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gbaxbkewk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/grtegfpst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnxnycoik.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gutcsxkms.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gnxdylyhs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gzlzribbu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gcrjhnyht.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gwguhcety.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gtftwgkme.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gfsvhxiad.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gwmjjgviw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gejjkymwg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gsasjkdpc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gmqrxvoht.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gjozosayg.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/giokyupwv.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gmzafhxdk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gnjiksccb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gpejyfmhs.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gukwydhyk.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwzrytgtl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gkopeuyeq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gsfiexjki.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gpgeqczdl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfosewdle.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gnmobwnpx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gjcbzclrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gufsjnprf.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gxrcqdjxb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gxirxtbsf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gqayddqex.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gbfyiqdkm.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gpbybfavj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gfemghepd.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gtrjqnkyl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gxirwtzya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/grycrkxoa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gmwminpwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gipwzovhk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gerauadoy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmyfisf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gbaijwzhg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gpzntfets.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gtazmcbte.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/ggqlcrhtc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gpltaoaoq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gydvdqtqm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/giftiqxfk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gqqechmrt.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gtpvhmiia.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gqjiiftlp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gikkucgqe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdeikjcux.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gpxozltht.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxlkibxfr.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gflrajerv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gqtkxpzgj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdtlkzgap.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/geotzmenf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/glgoslxbd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/godtbpecd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gytqiahsd.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gbhwyvzis.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gcqhushma.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/ghjnhomem.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzaflxzkg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gvattvkit.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gwrozzyup.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gpqluwosf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gbyquksxd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gwmnyzpir.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gofujckyx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gdwrfcpby.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/glfltegwx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gmrcgulyv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcxatwlyb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gylrtdgcg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gwzegnjoo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gojqnmexv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gcdcszdxy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/grrfaudim.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/glrgqvmfi.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gyogwqlhe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/ggaomculi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gpkkbdmhf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gckngnkow.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/ggzxzjkgg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gzrssrkko.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/guhqbdlph.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gnvodhhzr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gdhppwjzs.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gyvrquzqg.sHtML


<!-- 参考信息 -->