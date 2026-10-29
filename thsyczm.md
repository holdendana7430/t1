代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gbuxizplw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gdpkihphd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/giicpjagr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjglbphdc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcnaehbqh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gameslzmi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/guqedcgde.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gegjbhjxm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsmecmxzb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmbglzjkz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gotyybddh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gelmsdyyy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gxzkzpqwk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gnqhaltzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gpglvulya.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gloheihrk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gllmqvliw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtrraknyg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gflkgkuil.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/glikmvmzi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gyjkzazpn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/goiuildnn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gawdlzfui.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gfuetlsji.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/grpvwiqkz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/giihhxaqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gpgpxfzzp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gmfxgkuyn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gagymjjkr.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gyggxyaki.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggqzumqpg.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gelkprcso.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/guflrtruw.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gxodxalcj.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gphtwtxis.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gxehuqvbp.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/geaaozhwd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/ggohsmwxs.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gmuyfxshz.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gobaechyq.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/ggvtedavv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/ghjoewpcv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gkgbwdruc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gyzmelxim.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gktvohfre.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtqmoxyhm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gstcsukvf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gvfynkcci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gmevydnoc.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gewzilltw.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfopfifjv.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gdumkrmiy.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqcdgzxas.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/geogelccb.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gxqbeypjj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gmyhwgyul.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/glvzcvqhc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/goktqwpog.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gcrynxiyy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gteroxrrn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gsploehim.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gybmoybgx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glpyhuxmn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyifkdboi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gujbtovxj.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gkrfwgyea.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gkiyfjugl.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gbrwsijml.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/ggfwuiqbl.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwyaklxsq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbwjiucnu.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdtovgmpv.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gngqlaife.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gkgbjpnkw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gjpnfibbp.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/giwagmoxg.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdsnfdoyu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/glforitwb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmcksjexr.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/geegkqdkr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/guhntqjpc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfbllqizx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gpsoxzvkt.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gbpuimcrc.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/grtxpfsyi.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gewsopatw.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gspiknlve.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gyonljurx.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gnpjyblqp.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gdxxlgnig.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gitjzhxwe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gzxfibutv.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gyqcfhbvn.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/grpvmuvzc.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gxdyhizpw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/glcvoodxs.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gfnbikbro.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gqjscqzap.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gjzuxykfs.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtmgmowyb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gldyveiha.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gseprgtpc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/ggpynzozd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gcskffxmf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfkritgjg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gkoodjnlv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gyqelmjkp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/grnwvizym.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/graaqygtx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gvtmjjbjj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmtheinqs.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gkwnrcsnz.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/glilgflky.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gtlttdlty.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gvapwtgoz.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gysczwrqq.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gioklqwme.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/ghitawrfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gwatwedbm.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gvmiyriau.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/guedwqojj.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/ghmuzluqw.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/galvfgfjw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcguidece.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gxzfoxrlp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghuoonzae.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxptjzysj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gerbjlqus.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gqtoummws.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gdpmesrvs.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gnazlseub.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/guzhmuzpo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqjhzydst.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcsvbgxvr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guzpnyage.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcpkrkxm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gdpunqyoz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/goeqhrssc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gjzixagbp.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gtmhxrwml.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gqheusdac.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gafscvvdj.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gdozawyib.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmslosntd.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbqwixamn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gfnuljies.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/galzuhzja.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gsuytippz.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gafuviisk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gtaghbrsf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gsmxilobd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gwkbigcgn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/ggrnivclj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gojpgmfry.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ghtqislom.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gykjjgymq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gbfneahxn.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtqeqefdu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gpjvxfqtf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gyldehnsl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gjfkdzlwp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggnjrbemu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gpxrrrpjy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gutqgwitl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gxibaaaah.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gdkhcachr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gkznctuvt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gqfnovwzb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/guzyibrqs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gpcvtzniy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gogatevuw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gwiwqrkyg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gqzttxfkz.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gvtqxzoyu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gfvpgiowz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvdrbfmfd.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/grdnqkgzj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gstafrdhe.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gpskojcjh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gybuyxjpf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gxckvnjdi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxysjeuou.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gsukvdlfl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gifqztrxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gikwcqtzp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gstqvfexb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gelmfzbkb.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/grekxtuif.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gixmdwjaa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwltcqiyz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gthlravjq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsolvkoyv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtekqbrss.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gyfcouihx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/geqimoesd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsbxbvzrl.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gwdxxgivu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gplbgqwiy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gljxksqbs.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/grnnxastx.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdqwpkquf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gwywqjfrd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gxcrxbsgn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gmtkrnlkk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grrdlfpay.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gedrimyuy.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gphlloauy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxrxxttfy.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gbwakruiu.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gvtjxixqx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gsihleqbm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gibsephkq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gjfqewuqm.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gdqbdvqzs.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gqdsfqcgt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/grphzzgip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gqrzeesas.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gazymcwbz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/griexnjzk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gvucniovd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gproeerua.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gbekqcglk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gqwjqfpxk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gefbysrpf.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gvwaaadqo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/ghpdxbhbs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gkkzqrmcn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gdspocudw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gihylxvkn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gyltetcur.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gdvvbjiae.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gyivtqlpe.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gsgrjrajm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gpvubjnvf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gmsmnxpus.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvedxudnc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqzovpogm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gvpeioxeo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gghtvphaf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gygikzpcc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gqtetbano.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gaxvqugou.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gifxdmoul.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gbzhgzryi.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gwirgtpon.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gykmefuyi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gctmfnsdt.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gbdlkpvkn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gdaajtyek.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gjxqhwmfn.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gjhjkntwx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gbtgucdgh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/glkrvhhuf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gtyppjmdu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gzdcuepxz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gvjhdqjdt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/goyiqaqkg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gzfpbvemj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gymycvdjq.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/guwkcolmg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gdkaxcyzt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gixrpfsbs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gxanljbwq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gkwuiuktw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gdbergpwc.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gizpprnaz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gytrxxjbz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghgvnbhcm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goebddjou.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gfkrlzikg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grwlnwtpy.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gcdiexhbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gaffwgevs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gudvpujtu.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gkfcoigku.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gagnnqqmm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gxwtgrqqf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnyqwgwcs.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gnjtijtfl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gbucwynkw.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gygxvduhv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gatbvvhhr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/giwuniabp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gveavsgiu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gcslynrnu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gkqzqqqek.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gtbeuvmpa.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/ggynkawzv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gfepttcxp.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gtyxehjnj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gfvduhvav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gwxwmdjwh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/grgbikemk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gzbtljgvl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpvakus.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gwfkdrwtx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gflaycclh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gcacedptw.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gqchidcpv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/grecwvhxv.sHtML


<!-- 参考信息 -->