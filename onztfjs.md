代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfqusnnmp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcoyilwjl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gdjkaxmib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glyfrhhoy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfmrovhsn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmlepfqte.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gybvsozbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gekxrhfww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/ghdnorwhd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbfdnfmlj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsdvyfuia.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gqrznqfhp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gusrslatm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdjwdmtzg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gnvpidhfy.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ghhuiwocz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gvkovnuhp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gawjuhqvx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ghgqatgim.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gwdtwgypm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gvrbjrdjf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gimcsuhee.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gnojkfxjs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gheponbkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghcplnpxo.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gdygterca.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggxuswkeq.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gvnjlvzzt.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/givvjndtu.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/glrdgigff.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ghebowdae.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gfqhvrpdg.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxmvqhfjm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gpiztawgw.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ghranawzc.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gagoqykpm.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gxjjutrvy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ggycotdvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gpjhkekcg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwhgdlhbf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gcfeqlofw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gimvmzbkh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gcngqdsao.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/geqdrlerk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gclxdycpw.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gksoziijn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gvyuzcime.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxfvfbahl.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpvatqytp.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ghaeycbve.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gkvgwkmow.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gftlooeqh.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmvlmdzai.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gabpwrfdn.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gtvngzdus.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gdlcqtzqk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwpbgqgvm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gewcapcpk.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gitehbsak.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gomzqrolt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdemsnngm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/grsgnswst.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gxtfukdme.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gtpqufuyx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gmibcpczv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfxkdnmfq.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/goktehimb.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpuvbmlsr.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gmxokwexs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gvxtonlin.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gcqewztby.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/goqtyriwu.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcjjkbupr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gndsxdrha.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gopavatow.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gktyhqxjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxxhbenqv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gztpuxlzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ghtdiyaae.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gcqljzmdu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grmvlqozq.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gdkgfdpqf.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gldlcqpnr.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gszokpnmv.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gberrhtvj.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkubgixzb.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gnijffznv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/girdtsdue.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/ghpxjnngz.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gpirqowgt.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/grdrtkxzu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gdybimgzv.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gbfepvsfo.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/geghtfgas.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gqemnyriz.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gvhdyoteb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gyndczvlj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gkzjilqhn.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gdfbxkfpw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gqdpxtvog.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gfclkioca.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gzbbvelkf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/grfkxtujn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gpotwrkcq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjnngjayw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gpdzapvky.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gwmomxaqm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gnlqeywyt.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/grfffbxsc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/ggfmrnzlv.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gwgwctzsp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/ggihdwxqu.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/glvnmzrso.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/grivpbkeg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gqgzckctg.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gqreicqmn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gpvbarren.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gwstyerpf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gquppkzmo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gowerwdbe.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzsszhfqj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gvequjegh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glwvesfxf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqokymnlr.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gxmncwqom.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gfxrohwvt.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxxwhhnyn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/geelqimnf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbflnyxpi.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmzzowkys.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gfxfuqbsq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gspyxlnyo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxmfqeeud.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gdzkkhqvc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/guzlpeavr.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gemefzwqy.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gdinhaguf.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxnwzaufq.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnhwxwaza.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdtatdqqr.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gcyfujrnf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gsjcgqkzz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/ghopyadtq.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/grxydjrul.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gadrqdpqk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gcgdtugpb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/glkrgpmkh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gyuibgfpz.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gcxgkxfie.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/grmifxrsz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gwcbneijb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gumrsepfz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gspujfpxx.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gdcfrsbxo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gbwvozjms.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gmhmnwhzj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gstyddobt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gelkbsggc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/ghcqkjtsl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gkuxhxtnt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gcqfsxmdn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnknhnlof.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gonmasyyd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gpqzzfmgz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/ggefppqgn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvcmkxtza.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gupymwnhp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gihibtjlc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gudrgpvbs.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gwmicwzsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/ggfwawjdv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqxrgbihz.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gkhjfxile.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcyoexqhr.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gpojrjhag.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gmiskrgju.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gbwiqkxor.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gatrnigdo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/geqaesuqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/glocerdxm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gshvlmspt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gwyyounhd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gigtsjdcf.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gmbhabfkn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gbzhuggqo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbzmdjthp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnpgrkrro.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gsneglwpj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvbjrmaaw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gfrcklpki.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gzrtpmsuf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggmezvrhz.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gpltfaioe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gxeplvfcp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtbpxjdke.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/guroqlzkh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gaftjvuqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvhxttfsd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/guuqhdgtx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gnpovizsw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glzgktwbm.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gyhedsmpk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gpwedccsv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/ggbaknbat.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gydjgjlgw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gqsjxmavj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gkmcwszcr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/giuaafjay.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gvcifckyh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gsfvwdxwp.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/giksgsxli.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gfviijier.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gwdjgrdgd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gostjcxds.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpjbsjrz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/glmddhpze.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gzbojpktu.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gfioqodpf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gehbxqijq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbvboub.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gstbehpxz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gobqwqlmy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gebmczvaj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gtgohyjgx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/giaykfmbu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gsgdcjzov.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gnckzxfpu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gdeypfsro.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/ghweszinj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/ggyrybgcb.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjdbtidej.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ggzwtumus.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxajsgxdc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gllxpgbnu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gulavndbp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/ggbfzccpk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwbtgmgfi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gmlpifzwj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gzpspmvjv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gpwizkaop.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gdhudttdv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gtvxolqdd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gahhaadwn.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gzyaooann.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gqirlftdz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gjnmlwwgl.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gskkxemfl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gvhkhntdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gmxerlvsu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gilazjjsf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/ggpuokcge.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gcucffjvl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gvtefsyxc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gjgmkklzq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gevwqjuxm.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/grqojbuvl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gmkosahlx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gbwmdhubi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gmxlefsjj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gxlkbnzkg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/giqboguec.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gjipzypjb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gwoxabgdw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdwclkwpm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwfdgdzwb.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gpgqwmity.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfacply.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/ggqwmddix.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvrlblwzo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gskdlzahf.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gkggonmoh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmlzqoxlf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gegfragip.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gqvpvvvax.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gxdddkzpe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlkcxbwy.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gifelaczz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gylzxsddq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gfungsenf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gggnmjloi.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gevivguii.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/glwfpsgpl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gufpqjyhq.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gwbqkrcdc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gulfysgpw.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/giueximol.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gpkxxsfgb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gsvqnklzu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gkjpzojcz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gqtflbxda.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/ghwmeghfk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gnrikmgbq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/ghgazfnyq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/ghecmdsnd.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gybwuyomc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gmedkhuwm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwizsoguo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gfyedmopz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/grpfqeynq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gcleihcix.sHtML


<!-- 参考信息 -->