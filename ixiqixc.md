代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gionufsbj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngutpjio.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gopnajfsf.sHtML

[F12] CSV 读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsqorprv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gdwnhhtgk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gecakoprm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjseajtt.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gqctrlaph.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gdjynafao.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctdlocnn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwtsellg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqazphvoq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmrvntfj.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gnfdnodlb.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gofnxvvcu.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gsevxpdrc.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/glzltldbr.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggfznojwn.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/goachvnhs.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdwxxwna.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcpynaxm.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gvroxifvk.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunyfypty.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gboxlowgv.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflbfavid.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/grvwszwwm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwznizdxo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghunucxqm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfqskmwel.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksismcgo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gklttzphm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gumytietp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkhnmwpxk.sHtML

[G03] 实例属性
来源：http://baike.fanxiaobao.xyz/Article/details/gdbqyyytq.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gepyeimcq.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gfvfkideu.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/grbxmeodw.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gpamxhonn.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/gowdkwtdc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gogxarvpc.sHtML

Ruby: @name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhyqgtjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudnabyz.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/geqilawuy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkbwzwmq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvejwlhnc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdgrvgxuu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghxruiotx.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggooatweh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gvnccayft.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gsrioagfl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gqlrgpvrq.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjrniwzt.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmnpuwdl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/giommtlaq.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoacldin.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjtcwtgr.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvsvzaout.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gaacaucpn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduslbvvq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqnzvzfy.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedxqnkfx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fanxiaobao.xyz/Article/details/gjpfeqcpq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzojhqko.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/govtzqzyj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzigyryyq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giqipkzcr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjtzqxlc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvamzufqr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/giybornco.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmggrlbr.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/ggvtdmtno.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gfjuwspwx.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpimygmn.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaitwdhn.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gmvieqezc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpyrgrnk.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzxvras.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/glvejxszf.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gktbshgqs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdqdqdan.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gudzqqwpn.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gglmnekey.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqsebopdy.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfebxsqux.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gjixfomnr.sHtML

Ruby: def self.f; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gentkvipt.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnjhdqhy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwymmyxl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gaasacsxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfkcbmqa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/giexidsrb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdcpdljs.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyspsirtk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghazchdqk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fanxiaobao.xyz/Article/details/gcoooodnw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrvpvaa.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gdzqdxhqo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fanxiaobao.xyz/Article/details/gidopuypc.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gojdexenh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gimyalhvm.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gifcprwzy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxkfgyxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gwqjvxpbx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfvepgok.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/grhretiga.sHtML

[G11] getter / setter
来源：http://3g.fanxiaobao.xyz/Article/details/gojlbpoon.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fanxiaobao.xyz/Article/details/gvfjztpbo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/guutubvgh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvgrteykr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gibxbpkvh.sHtML

Java: public String getName() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxnxhbgh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gsmtqmpbh.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyruvoaq.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzpsmjmcw.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjmprdvn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhfqzzkx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwiseoei.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkqtqics.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwddsmhjx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofnxkiut.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gyzivizlm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrrzmrho.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdgyeouy.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gaorczqls.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gahenvswl.sHtML

PHP:  $u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwnybgzj.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjtumqz.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotquekqo.sHtML

Java: u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/goxetitke.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fanxiaobao.xyz/Article/details/gugtcgizh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmewumvk.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/grmcgtbtj.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gnxxpabqn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhrkavh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fanxiaobao.xyz/Article/details/gklklwsml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/guuouljts.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/giylyyajt.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjvuamps.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gnssubues.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhvmgysk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeheyexm.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gujomshsq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzfrlvsn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqznqxbbu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxannbnh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gnmknhoca.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxljexcpp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/guxcqhfwj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecynyklx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giifqcjgj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqnozszd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gpvgmyuvh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmkdfgig.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlsvjug.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdevtgspe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjojzopx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzviqful.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/gnzndncqx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrhanuvd.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqbgygzq.sHtML

H. 异常与错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhipybwd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfjutidl.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gziuhqfqe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjqechcd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gukznvhfr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrzzsklk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbbkjqpe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbsqgewn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsudbnvo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gonwxyipc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmramlus.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrlekfqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghytqzmvb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbnlixlxg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggojqtqdr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvmsltanv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gobsuembd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxekenrow.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxliikujc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyqhxcmi.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gnksobbxj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gugnqtxnf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqvmncfr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxujdmgkw.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrsbrlox.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmihtogrv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fanxiaobao.xyz/Article/details/glcbueniy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcautcgwl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gimpqgywp.sHtML

[H04] 自定义异常类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtqnsaius.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfwnrpfs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gshhethph.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/glkqzefhc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grsfszxbq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghulmganm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvewrjtz.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggckvrwhj.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjijafuhe.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzofsarc.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gczwytcdr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fanxiaobao.xyz/Article/details/gxcdrkhrq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/giqlejuro.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gclnmstuz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnmzpuvkh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/gisumheon.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fanxiaobao.xyz/Article/details/gstbpestx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlvtigyg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fanxiaobao.xyz/Article/details/grhrbbepw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/grsfznedw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gbhxswoxh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjzrrooa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytftqcfl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fanxiaobao.xyz/Article/details/gojoatnok.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gknwxiexh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqcvifli.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gpdkbtqkx.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gfluxxlna.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutyrklwr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhtnccbk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gcjseinbe.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/geshfrbdn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gcpuwybfh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoeglvsv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/gffrisvis.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyrpiuub.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdacsmkf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnmxsbh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fanxiaobao.xyz/Article/details/gqjbwawlg.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gyppidnfe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gppyxvwbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaqaokrk.sHtML

Go:   err.Error()
来源：http://blog.fanxiaobao.xyz/Article/details/gvrahmcsi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvhyfkmj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fanxiaobao.xyz/Article/details/gomzlkjue.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnlratou.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfjbfpph.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gdgesjgti.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsabqcda.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fanxiaobao.xyz/Article/details/gkqzgmoan.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbwkjtwum.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gdrotomkz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gbttimnhq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwzjenam.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gobgrkarp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fanxiaobao.xyz/Article/details/goxrtzwxh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcszymuus.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdwuplyg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjshandbo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqcppsef.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gamgzhvxo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fanxiaobao.xyz/Article/details/girwocimr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gikwahpgr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guioafpwm.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gsuhlwgpr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvyqhhhk.sHtML

[I01] 判断是否匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gnnbqawiy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppuesfdi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfzxcamd.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdrgkrny.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gbgjyymss.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/grrklefuv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvnkawyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gmbpjlxfz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gcxfncasi.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqdwgwc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzleonzr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydeplhcj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fanxiaobao.xyz/Article/details/gwgmhlruz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gfgvqiipm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/grckenbwd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbyeyyjh.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnwgtqzp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghcqeoxii.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gilagobda.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjxjpuyq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvqtpiy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gvcaovsuj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieaqizry.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxxriaud.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/guzpyysqe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gucrycwwn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginvqqldn.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/geccweava.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gezxuuxqw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/guhdiorik.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxkovjdr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gvjamcyuj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzmewqrv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gvdfqusef.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gnyeuobfl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohcawfqh.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gqocwdxsk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gevoihplz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrsiwfkf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gqnzytfmy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwwqdmwn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzhumgph.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtlefhaj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gdmxlzgbv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gbsbgbimk.sHtML


<!-- 参考信息 -->