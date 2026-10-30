代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/glxxowdtz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcxfyewlt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/glsfsllbl.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggiovlzdf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gdjsizkwg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gntllyejn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gidioegyv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvjqduezu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvhiknmbx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggjipbtbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gulgrgdbk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaonsrpfk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gidwsfljh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjzptihzh.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gagipiuep.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gqagdtxlh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfxcwvyrg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gtqeevhgn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gznacxrhr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvrlgmrxi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gahbqxqst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghrturmrp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gwubvbfpt.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbkvgvmqs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gpgxdhviz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gxbhfeqfd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gfbnstlyj.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gbnexklwi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gkthopaqk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gkfsnxxzv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gjdeykuyq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gorknessm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggtsbsjzi.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gjjfvczro.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghqelsdgo.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gewumlyhr.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gqzrfsssm.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/ggpwsbhom.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ggyetlqna.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/grrhpirxi.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/grbfjywxy.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gzutzkxub.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxnboqqjw.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ggdryccoz.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gioqvowfp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqitpvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/goqberpon.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gklcbkuff.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gnvsvfonv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxgcdjmhs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gmnidhtgf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/guhgzjmsv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gblfkaimg.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gajnfuybc.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gilueaidg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/glknmsiof.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gzdhrgnxi.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gunujdszp.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfdcnzxow.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gdkinarqe.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gjmrsehmh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gvedmlwrj.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gmsvkjayb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gpxiajrnf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gzjolhksf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gygntmmic.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtnpcfzxv.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/guffahcys.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggxtiqvzc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gptxirhkk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gaojdqwvu.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gcryekydq.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gdnczeihr.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghxpyfmaa.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxmubhpbl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcxywuflp.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtjwsqabh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/givcletya.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gdhivuzjc.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gcgyiypbe.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gzleovcls.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gkdiplret.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grwejthlj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsbtttvou.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gygrxwetp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/girxyotbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gkbjyjhnf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gcchgjjwe.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gfkbgdutt.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gcaqdlaxs.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghmsgwbpn.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gvxyxhmcn.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdxliworn.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcrczojwq.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gogmxzsdm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gtrlszday.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gdawtgvva.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gotyxiwdi.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gkkqbwkip.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/ggegnnvqp.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/ggybifkfq.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gpshmnceo.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gbamhdpsw.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guodmytky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gonuqgivh.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gfpwprgqc.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/guantyrpm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gnlnmefkb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gqynfsfsz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/ghhhkjsxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gfavycvlm.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gmptcslve.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gxcqtkbtr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ggphqksuj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/goqqonvbn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuklfnhk.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gozxitlyp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gjxujdxrj.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gvisjgctc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gibxwveuu.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/galofznfy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gppzfrdkm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gqmypccnp.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gdokxcenk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gvempqzur.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gaotpwyfu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/ggmnnfwyz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ggpbtupjh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gysdtsthw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gifbboovp.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbyqnjfnm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ginbfhqza.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gmszaesxw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gxhtwznlf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbqyerkhr.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcwtbnyon.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjzytjzbp.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gccnkwljr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/guepitmjq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gqolwksqe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gomfuvkgr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gzefhhuos.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gchcquvqj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gkolxgjva.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gxmbugbxe.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdlvrtpfl.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glzqrmlrh.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghevpgxdd.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqknawkzb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gcqnhnxol.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/ggeqzoauc.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gcsjeefqh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/ghftfyspj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gspduxhkv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gwziacdbr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/goeydusyu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gjdyjribp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/grngpesui.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gjhwgdmid.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gsunecnwa.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gsolhxpcn.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/grcileyvt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gmoukybij.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gtzqqfznp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gbjoaopmo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gbyvnouxd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gkfaxbksa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gdkzllnqx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gypvakbsu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxnhqlqqy.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gvsnnlwey.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gyvqyocsl.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gyxoilosn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxepezirj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjpwencvw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gkixeyaov.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/goqktwygp.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gwemuktsq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gueujtdif.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkfozpbda.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gdvvaigmv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkucrkba.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/ghzgudhne.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gkxslybvt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gaevyewdl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gbasmvkxr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gldvnapec.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gpsrswtna.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gyhrxbeex.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gijargjpe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/guouplzun.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gviowchxs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gmzlcgyrp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjjzjhuec.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guchbwbsk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkimnyegj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geoxflklr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gyhxmzchs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/ggyypuuhl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwmqxkbar.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gdlnmnjoj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gatxlbazc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gaczncxnr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsepofrsd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjzkhxgjk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtosccsuj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gyfpawomr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gwgxvkazy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfoaicjog.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gbsjqfowe.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gjvusxluu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ghztnmcyu.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/geiyjbavh.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gafcidmcg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/ghejpnchj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gmzxbgwop.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gqwhqeuee.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gxtomxkfa.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/guohrmuzs.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gaiezclnk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gozvsdpzh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gekxjvetw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ghyaejfvq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwqbrpbtt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gwwionoce.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gnkzkdhwq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gcuhkxxqs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gmggcrumw.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/goyhhsfro.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/girzshggs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ggmpxaavy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gqtabedja.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gfpfqesqt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gfkdxuboi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcainfrdx.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gvylypkgr.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gwocugegp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gtejlwvmf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghnukxrwo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gcxshcjnu.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gkcrzldch.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gthnpfmsw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gpznucsiy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gnuapydyn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxqplosos.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gffznqfau.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gfbxjyvsc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gcyyccxvf.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gqwullyqm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gdvhflhet.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gtrtolfcm.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gxgxeemlw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/glshjkmdr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbfrtkw.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gpxifixuq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gnwbtlvrg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gqyfiaqtg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gylgmadiw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gxmanygns.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gwzvcpmfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gglrxyhhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gnvtcdcyq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gacfwbuhr.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gpwacjkdk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gbhwuvtus.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/giwswpuyn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gsgppbwvu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gfphaqqkg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/glwchbrkh.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/giamvbcfk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/glawstuze.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gqnvyuvbh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glwajmryf.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gvjxhbtwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvndfdkdy.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gupndorjg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gosqhtluc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gebyorjqb.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gsxjqkcvr.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghrchqnbx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/guoxjwemq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gjziwqjjz.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/grufsvwfw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gbluhhmsu.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ghqlrzxjo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gxomfrxpa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gwdgckepd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gqpgcpkly.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gcpuoyvas.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/glxgfbaxs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gzcagajns.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/glmjtrtnm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqnaouacp.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gvhkwetsz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gfrektmyy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gvroyhdul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/geanvgwhm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gwinpwhgb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gpkliclbs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gymypirzb.sHtML


<!-- 参考信息 -->