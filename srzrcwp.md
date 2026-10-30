代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnkoieqhr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwfadungk.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/ghsbczcdm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geldhhmhh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gakociztg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gozfwdcqd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkpwzrlcy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gmrltybmi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gezzqwzaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guuawcbaj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gqgppfxra.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gnwbiicnr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gesantvdy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gijiapkmr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gzhuehbxr.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gqtupvxfj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gnfyzvepc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gxwmjjevv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/geiyzziat.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/ghabmbcej.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxqpoluce.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gcfwdrhsr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyerrnwaw.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gdxitztnl.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gvhxtpdoq.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gbsoylsyr.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ginjlwava.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gsfcosykh.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gclmbhshm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gdnzaypdm.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/guxuyezuq.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gwfksgjwt.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gebgblgek.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gewgykvez.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gejzhykgn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/griyqgtak.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/grwlythfc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gzlhkmgqy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gptadyrta.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbfbjrqps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzqqfscvn.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gadudaope.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmbkexqxq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gmokthbco.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/geurujbvv.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/guzstjlwq.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gtzrrkewa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ghrgowbgo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcgmauok.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdxqcsrxm.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmxmtotyw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gcnhnmxsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gulyqmteu.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxiwdcqyk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpvzdspuk.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gohrjdpjy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/govhwvrbm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gyqwirjlx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/ghjqccyej.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gwcyvapkf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gmcxafkgp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gwybazosr.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjgdguodo.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkaeaqipo.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gshcsoatq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gbzvnkrqa.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/glivzkhiw.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gxgasyapp.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gcoztjygr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gqecxbxyl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glpyznwby.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghbgxgcbu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gehmwxlcc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzfgzlqzt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gqgblewqr.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/ggmztewyk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/guyxgikoz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gqzinsaqq.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gfqqaktmh.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/ggaaimaqh.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwapasphm.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcckndlfd.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyovhmvae.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/ghgaprvam.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gsoiknxwd.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gjiyngtxw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gocatuvml.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gqyrspigi.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmeuuncrc.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gunaimion.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/grfimflya.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/godptpjyh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gyocqgmsl.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gkdkumqlp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gepnapxet.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gtbqhwbrr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gfenypqxp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gjpjkophd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/grawfhoxd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gnlhcwdch.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/ggksqzyte.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/glvfrsnjr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/grxspjngm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ghsrxudyh.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ghgnpwpxa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gldzbhxrb.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gocqnntuy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gixibpaxy.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gyagidhne.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gzhvaaizv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gblviburh.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjzhpsypd.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ghtigpofl.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gvmeqptaf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gcpujvetv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gjpfbnrtv.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ghtrqpema.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gadmbkwao.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gblagtttp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/grtngmhfz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gaikjbplk.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gjotuogsa.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gbuoxvqig.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gnewoowgf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggbtkksqv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gdjzjfaqi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkipqiepr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/grlhykiej.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnvldxcjg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gyfxtunaz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdbegdfse.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/galpyqzjj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gupbvvvqg.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnsothgkc.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gjgrfmguu.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvpycjfsf.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gempmoecm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gnyhckjkq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gbxyisjul.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gtixcmwob.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gdektzbke.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gqzsrpdgl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/geursqzbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gongiqtaj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/grnbbplts.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gbmqorizz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gsxlvnxnr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/grmkecksq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gvksfmjya.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gfvqretpi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/ghnktmdmn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggohwducx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gwcrtvqjp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/grctxdgeh.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gxymhhvbc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gnfnvaaoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gjgquxflg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjrqwodpb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwvsxxsql.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/ghiizfgne.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gmrxexvhy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggejaiyvv.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gjziassxe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gdjbqdtdz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gknytxbgh.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gyqkwgazw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gmzpycbtr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdbghifcs.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ggrhzpadm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gomvpoypf.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gkddmezig.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/grjkeemxi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gjldanmqr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gyzofoohj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gsjolwoqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gdrmzidxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/ggwimwtuf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ggrihziss.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gvtmkbusr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gnjeioubu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/grjukzbhj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gvxensaut.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghrzxqtbz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghqdvjigq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfadrwley.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gnopebdwn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gipvvdotz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gznxyvjnw.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gxhignwtu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gjmpjdjep.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkpqahtyx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gexoxwuty.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gqreumssn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/guyrcctaj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gfbdtiyvf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gloceuluh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdcrfepba.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gsidremmb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/ghjdkbjrt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gymucefxy.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcmknkdeb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/geobwrron.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gqfwzicnb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gzxwwtwho.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gknvqmukv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gmzrlnyhn.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gtxqcssbd.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gyphxaxrs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gupebicln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gatniwdmi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gaylipmup.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxasscda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gkwtzmgco.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gqhnhibqg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gvxfvhxvf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/geqxnjqgy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/ghyxgewrl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwzdhwozn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gvljflsxn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gbokmrqlu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gqqftnomj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gkdddmech.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gpvlfpftn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/ggqrxfgdj.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gqarjtqcc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/goplblyyy.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gmnyrwezx.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gffshqida.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxgwtyxts.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gszcrlhwb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gabceiywt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqpxwmrrq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/goxvjgewp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gfisvrlob.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gtawrlnid.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gabekeqxa.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gtjobyvrk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/ggdxvnusu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gxutenrsd.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gcqsjhpbk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gfiabrwsw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gecqexkgt.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gehkretcw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gopgdaoeh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gajavzsxf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/giiedkjvz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gfggomxvr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gzazekffk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gisluqopm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gamdndcdj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/guvbbeqzm.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gmfbwwzsz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gptfaoson.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gpuwflrxt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gvzojvtsh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gssbflckx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gzaekrnii.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gpmjwyliu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gpvvxbhdc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvnkkjvth.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzqcmblmq.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gyuybepir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwyanlfkj.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gflinxjzb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gckoykcgr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/geetwgiya.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfilvbiq.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqkodog.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gpyputhxc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gjiubajam.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gqbtuqzzn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gxhygbfdw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqqdqxwvq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gjiiihuyd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gyrtewyhr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/grdbnprdm.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gqxarkdez.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/goyhezglc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gvollwiqd.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/glwfjszao.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gysozwcsh.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/glvoknhba.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpwrojjav.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gcjxfacar.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gtnqrdapq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gwszppoln.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gnfayfahq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gzepdsqln.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gtbqzunrd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gcfeeaeyl.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gjvkfwtvj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gjnlzlzok.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gjqamoiir.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gmyjlcjhg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gvoktlnmy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gbibnocnf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gkfpiryus.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gjhraazrr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gjkskkuxx.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gwebmsepp.sHtML


<!-- 参考信息 -->