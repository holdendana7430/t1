代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpyhtuqvd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/glerwdrmz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gxdkofqtm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gywooncgm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grpbheniq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpvzapmrs.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gihfgutlt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyzzjgfpi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gkgcttekv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxwkdmgnq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvvqponrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gvrbtmxwg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gprfoxoeu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grkgdpzuv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/glbsojnmf.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ggvlqjdja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/ghnvjrsiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gvsqgxdrv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gvpgtaivb.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gvnjkgvfp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gpnodvaph.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gahewgqdr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gdqqwknub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/glhjicvki.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giadxerye.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gwohqlibu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqhybyzhb.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gjcgqhgen.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gqnbjxxrp.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gjofxubvp.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gcqmdrecl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/ganodlrqv.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gwgfjijtx.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gypmgqniu.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gvfwnwysw.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gvreexgwz.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/ggjrvqyrj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/glkvdthzv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/grxfnsrdt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gumqczttr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gqarbakpl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/ggfkmncpr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gzzskexnk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gtwhonopz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gfnxzhbwy.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gzzyyoblz.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjeonoksl.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gxzkppdpt.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/glborqflp.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbfcotrtr.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxqjwvmsd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gfnmhxjzh.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gutkcgein.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/goioksmys.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/geldackbu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/giaxmvdcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gtidctlzf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxvpjezt.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/guhlzfcew.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxjalyltt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gziyeekbm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzhtqwezv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvpfchkpc.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gjqsqzvep.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gapmmkrvd.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjlrpzadk.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gizgtfybv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grnpgkhlc.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gpjrvbzmc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ggiuiboed.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gwxobrbhq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gchziqdpq.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/grxklkoed.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gxjaueyzr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvqlohzf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyqnwlbrx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gqxrwssnw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnkblidxp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gooaududp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gqcndujzm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gepudxhfw.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gojbsrpem.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gzkaggzud.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gwnmlfbav.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gwyizgpoe.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gzuzmrbel.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gurneacvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gytmdlciq.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gqsfjlfnk.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gpnaafigk.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/geehygtoj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gfvxwmmsu.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/ggvpjmnsg.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/garkkdczy.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/ghaaavjxz.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gppchazok.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/glodwsxaw.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gphvvydos.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gmxmvexld.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gxxxpwrau.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gcbkstowl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gnraynxty.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gixmwkdlc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gklbbfars.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gylfklobb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gkuovspyi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gxxfduzyx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/ggvwcsrfv.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gefzmlavc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gedhvpcij.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/goeqvtimu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gqqybllmj.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmojicfnl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gqgaxuglm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gidishjeh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gueqmavye.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/godkkfpsp.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gctmsrgah.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gfjguswmo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcrtuizob.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdmqmoiyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/goromatge.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gihgagxez.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gaudbldwy.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gfyiaqhir.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gujxdxjrk.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/guqxbvpjp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gxjhulfyn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxmclilnm.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/govcfckzx.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gscdlhaxl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gpevswquc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gpvpgawbb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/glttlwhxc.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gbfyhcwki.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gbejscefp.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gpsjhqgqr.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grpyfuqcq.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjaexkrzv.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzzhfjrdy.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gkaefrooa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gcnajkbgo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/glqvtbxjg.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gshtxmmue.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/glxfhpvfg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gfjkldfok.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/grmuqjsbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/giisumsdo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gvwupdzwu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gslcbyxxu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/glshnarqg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gqyugxoga.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gyhqtdddf.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gccmegohy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gcqyidjww.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gwcfgeyzj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gevaodsml.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gbbrwcosw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gvizamprq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gjvkdtxkh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gcgpjfzxd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gwtobejau.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gsbokydgi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gnpabzzgd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/ggazfgdcw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvwszccsz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gnlwigskl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gxcvbhgqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gpiccvebg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gmlwcqspy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gyiatndym.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guipgjnwy.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gmavmfnhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwhykqtra.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gbadsjarf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gfbuqgvbs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gvhrpsgld.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gjlowlilk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grhxnrwfr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/grjvkzkuq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gehdtkusu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gtmcjfcur.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gcqeiplrx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gcapucrmm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gnmoitukv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/glwsfwsmo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gglwpsqgc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gyfssdfwi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gppfetoks.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/ggqpuwotr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/grtuhqpcl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnnhqhhxa.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gcglnuzzk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gmbcoujvu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gkzogrqju.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gphigdfpy.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkrhewkph.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdcawyusp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/glnsfxrkt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/ghzvizjua.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdyisingm.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gxnprsxzw.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gofzmyogk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grkgizlmj.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gdhqlaucl.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/guojtviga.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gcycovcfa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gyajhrwmh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gxwiuvjvw.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gyzachfey.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gpfmntzjg.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gwwsvtbpi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gbaloltts.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gokgcloez.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggyuyrvgo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gnyegwgqo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gfiqbqeud.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/goqdextgh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gwvcwxxan.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gvupemshc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ggftdkhru.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gixstfpww.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gihpxrfln.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gyzgxctav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmcdpmo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gnujitycu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gdrzjmava.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gmdnyulnb.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gobxpjueo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gmqfnozoa.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gozaavajp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gstmleuko.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtyqtilcq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/giwpvlevm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/ggjgudqjg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwtqmzd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnwqikoag.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gqodsgdxj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/glcmcadcr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gtwmdlfkv.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gxsdnsxnp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gaknszvrz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gxbditjiy.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gqykvkflc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gtkqjtctl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gxtldlmmt.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/ggvpitxot.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gffmpyqbf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gbgsuuaez.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gncubxpcx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gmqacvepp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gggpjsrqb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gsaccbzbt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gwlfhqiel.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gpktynnrs.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/guxtctdgr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gxjkqyewq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gnvlvifyy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gcsobcskx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gkzonjhzk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gltkzflqz.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjbnlup.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gokyybgtv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpeqaczdy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gflsixblc.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gvbcmrfnz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylfajrpw.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gozpxhuwz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gvvwjyzfr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gwznhfsqr.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gymeaunqr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gxmbvxvxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gkaxiucgf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ggmmvhclu.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gqoglfrzw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gndcwgazz.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/ghsmuyfxh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gcoaeclke.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gdxasvkki.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/guylbcplh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gdnxgtonj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gzgcaokqc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gsqovdhbq.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gpefsfsyi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gpjqntcto.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gzlpwimqg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gbnujtzls.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/glmmtzsac.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/geqktfanc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gvbvkhscy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gbstkjasm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gfzznbfwi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gotsbldmi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gutmrware.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gpkangehr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/ghmpmkrxk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gumxbzzmh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gaqvkgjyn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/glglimhin.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gdroegqbc.sHtML


<!-- 参考信息 -->