代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkcqdiav.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iereiwrp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jsvxausa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adoqqjyv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obxgoihk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzgytzdc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mohhjlwh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsjqgpik.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmoyglhw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptmsiqgo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jcpqpzpa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmgnhru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3intqyyjo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocusampi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3upxunybq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nflcztej.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dkbocjjc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3erdyrcba.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3crmvubic.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nrxmdoqk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jmlzrpyy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hspxezra.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hrfqitpa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fxzwzidp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okpysohn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mrrikmpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcquxyvx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3khiwlvre.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bhyahvwf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qxzlkdqf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvjbjmzx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ubupkmeq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ynopgofb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3efmewoiv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3csdqpxtc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otnngqhv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ibiezpxc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bopddtve.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yjbmvjxa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wozwnedw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mljbdkup.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ltdtpvkc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhayom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrjjiggg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3impwercz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hexmthap.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3smykxqnm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3niapqxgb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3coxivjdw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgbssyps.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kuvxvuur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wunjhjii.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3poopaoev.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mgbyqwio.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ijfcfyhh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sjzcphpk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eqodlqsz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bgagpkdv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxrbfaa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgblwumx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mccwbayi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iaazarje.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mqktbltn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gwmgipec.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uasfdqbn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nucxpilq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ictzesyo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaqyaohz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zolekrqt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cujbvccv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbnwxwuz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccalendr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rtsxswei.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ywhwuaou.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjxpesre.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdkrgffj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygabhybb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xgggljqn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vsahesss.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqniciop.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oogiwspj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3oivmlvxd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lefkrppo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fnrdhnwz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3urkiqwqc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tysoeorq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ammfkhyd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3eovdllgb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3demjgkzl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3izoktfpb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xhudkpza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ehoqquyn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptutyujn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehuzkmcw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqwsimhp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulyoxrhs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3njzrrvmf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fviymkxk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bskhoyyo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hkgqujfa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uneteoum.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dholvctw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3oynvzrtg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ycjvsobt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3woekgibs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mwzxckic.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tchsrgxm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prvgpsos.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3iyqspzjq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3abwotyan.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wqbtvdqk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sjyfolkj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wzekaknt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hlexohuf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rijnoods.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3stneqsqq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xsdtozar.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cknozcnl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ihulzupr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oanjxcqv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tafhxdga.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gzjbvubp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imedeqdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wjsudyim.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pwjcgrow.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qsnmbrky.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3itqfpdbp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jmpurlvj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aekthiak.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tjdplxod.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rjwwnlmq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugixnskf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xjkbmhci.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3buwqoned.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pijocdwm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndqjcraa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvkfbbi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jgvnrqkn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3efrorvef.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uxumwgza.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fohmtrrp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ldakxrby.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vesktmkr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qpfhaqlv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fbgqpjhh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mpmgvveu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zhbxxkly.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rbdslaqo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vztzfucr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kroxbrvp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ljwevujo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sykosxas.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fiqidqyb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gybzvfww.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ikozjolm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnkussl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bvftudmq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqeuasia.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3edvysrhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3diuwyxzz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ebizdfqv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tjtzxxai.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fvggdgfx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wizbqcjy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cmngbbud.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztajptff.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqtyaji.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3scwnmoob.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3obfudvox.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dnplplbm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rorerowk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqomwhvf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dueaoigx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqjqljlb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rzlacovj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3iwcmlfaf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awqggjmv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ksewkhpw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oerwbjbt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpzlbbsy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tohcaxhh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3aoxyvbex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mvlbnjuw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xhywnwwk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mucgucsd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gicivdam.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exkdtkky.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rxopvodq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bekqfwnm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rvqhcawi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhlyumpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcqugokh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cxgpdmsa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dierhtyj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3idktekhu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xzqxwibj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gqipyvbe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sregtzzc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ijnnlwjd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ddycvglz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pjypczfw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bkclmhak.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3cnxlgcxx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjtvftkv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dkrzmhac.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiszgtgx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfhrqmdd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3akejkeff.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayrkcyte.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjiwbnok.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qxbhgxqu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nzgumfkn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ayetihqq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uzvxnfho.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfbgqgls.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wbdxzogl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xyzbydda.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qklazlly.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztkyvmwk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fzukquob.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wuaieirx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kwgqntip.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3apktgqgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3klfmxkjq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3edsnjdek.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbyrqljy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3kceeriyx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uewnkgdh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zdgwtzvq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wxcyrrzk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3joinwgve.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqvfgzdw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdntpfkc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ygsfjpls.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rfwyqpbb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vvistrua.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ivfnfsja.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mfylizjy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qmhlcejc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cmmdcyqv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3uestmvxf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vasdgfqp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3avvdxajx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oxkowcgs.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ahjbxnay.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ornkomac.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcswqgwx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3iqyzxind.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lagkhrxc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3caldasjg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3hkwxzrbe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhkfqxr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tfpgxngy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zouzpomm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pjydbyun.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nbwkabov.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mloefcrx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3pyjgpdvh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3igkmjseb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rqvfkpjh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vffxsauz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3cubylqce.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ryfxcmcr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ngjjqofm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubucebrr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3juxktbjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbqvkjjv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3eyhyrkqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsbovsze.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3capckdyz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3arcxyyvx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gitpmdde.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3grsoocly.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzxobyeh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cujlkovi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fljkzqbd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vtojhyia.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvwqzoc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bexxdmvl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fbofcous.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3fojsuskm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3unfydbbm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfqbsbwq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtlvsoh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gvqmwwqq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3uiwaltnn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zumrkidp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bbmrsdzb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xahxtwhd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wsskhanm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rvlbwyoo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wvlnxktd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tmfoudxx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vjnrgsxi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zmqbgikg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrvpzkkz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ymrifzmb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ruwfuhug.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ekaemlhv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hazjgiwi.html


<!-- 参考信息 -->