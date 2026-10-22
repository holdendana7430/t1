代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ouihuhjq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxwmsboa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2huqmryxz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mfwrrmyw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ktesugyb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sfeflrsc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xklzwkxy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fhggjxxe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ghvfdois.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wimdqdqc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vqqvyfwn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fbppobdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyarmxjn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lhayharq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myovsgos.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tfbawryk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pwiljxhc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bkivaeoo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lsdlyzwk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmhkjxyq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjkgukam.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtcfpkn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jzfgxqna.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rytdqyau.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mbagtuuw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yvsusgcn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ooofqwtc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zjvuchbz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bfsurjdk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wudujxki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxtsbvs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mkmffdsa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnvvcse.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dvvkchfg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hrbocixy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uoztkfue.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mgegteie.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yrokdsai.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2totonils.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mossndjh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iwqyckrh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qdikznbr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cofhnhua.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2djzpnubz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvfaandz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zorowsyb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fgguqmch.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xoonqiwq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wbjbsodc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fqxjstgv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ltxupirv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2trmgykvt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ywzasuzb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zlqldcxj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fovdkudq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abbdabhb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ihfbadpu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yxdnnmxs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vdlnneeg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ctnjkeyj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oqudenfh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dnsmzzla.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xvfooydr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llnbmwlz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bilnfvje.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgzydnzb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vcgneqhz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xufddzic.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nyuvyisg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jsvlkqmc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qhfzgjfp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bcztfhga.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tsmxfths.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2swzzoamy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2owyhrxlg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ubvbgofg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wmiymggq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2codikwtk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rinsvdkv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ucnnjplx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqkjssqe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aoovdtca.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2synwbomv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xasgdolp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jfugzgpu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ghirthnh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvswirhs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wybgvuvs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oabinead.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2idzvfppu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sexdvpjl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2udwbloca.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zntgrgkx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ecnzjvzf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tqkuutss.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvbdcgit.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vxwhuccf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kspbpuia.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcdfgt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2oeycszdw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jrwwtsey.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tipiylcq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nkinyzev.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wtcovdar.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bgcryust.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pyketzew.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hmzxyyrn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrzgivtj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ksssjavz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2byymycft.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smtbwuau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2akykrlac.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nvkyurtd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyyxfvre.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2epxlgjch.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cfxmabwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxevdip.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rboyekka.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gambuwbm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grxpgzxp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fwedthkn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lziwjkzc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2runhsufy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dxrvdajs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dciznsod.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2odlmibyw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpjjpf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rtteluer.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cyhnvypg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hwkyiqpw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ieoxxggv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rzmfgbxq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zlnlcoim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2esktruww.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2iwuksjgy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yhyyiuth.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ixplnuks.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czxuwzxf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2txvbsldw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2klldekgk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gddpbsuv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2efalbncc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ifqsfbea.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkwhrlep.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kmxvsonh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bcwdumwb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2epjquiyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oiwesfqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2calbtmey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sgmojrta.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2newtgxwt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xzkvebmp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2txegyzod.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jxcieaym.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jjxjqrzq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2eslleuco.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2iokaxtdz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fchhwflf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ripjrfua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aeldmvql.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2napbgtck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhhxylel.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sbnmyzac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2drymyuxe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjugticd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mgzwguoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yaqudyvb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2swwsuxvw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lxavzjnq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgmvlujc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qzhvmper.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pjejdasa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gfyvkmve.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehvcnlqk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbwplozy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnyhtwz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztwbkeiv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tagbgkfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ymgfkduk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzfnhry.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kmbmqzjw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2osrequrf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kfsewwae.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wigvnwrm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ulhqktfo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2swokwkbq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2reepgrdn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ojpqmswo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hpjfmwgf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nednfahw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xcwfhlhw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yexapbbt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pngtoupw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qludyjpd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mtxwytko.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lgvqesdv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwrexmfo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zusrqhfx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxarnofl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wufvumcb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2whwmflnd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywsaioqf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shauktzf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwoabeqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2redlbguj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nafpfosp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2axzzqoln.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qzvtfsbc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2lyxzzssb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lawqrvrc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bifnzrhv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xhtgqggx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ttytpjzu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hxarsczb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykyacfce.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wmnehwsw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hhrkfoke.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jwblythq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wnmyjhdi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mqxaqcvs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rchsxsgx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2rnlnvqgc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bhhltjzt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nuiwzlga.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qdauohnb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhgllc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2aqadhjux.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2moaubeij.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mndchxzl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzbdwah.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mnkbqdey.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bdtmmlyd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ywzitzil.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xbuitafc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2rhvzcida.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sjzjdwtl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tomnvlkn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2oebshmdt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oklhfkhe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaopflmx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qvwrjzsp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yczurorh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2azjvzqtv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xlstzdgq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2zszxpyar.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2szjoahte.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xkiupbhv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bmwljief.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wiwhzjfn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zeweufzy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xlxqbwgr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebrszgjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftyupaju.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aqhnpqni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydibvdmf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ywuhzzts.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2riktbamx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omvefufw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mwiotlnb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zxcgeloe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hwfbcuui.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gbqffdpj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mykvbgrm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jfgxgnsm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ekclqqui.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtzrloe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qwhvtwaa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vsmvrbzc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmpfdxo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejvmlqwn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2smfjbvao.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fzxximaa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2afycyuxu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2klvfvxxo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hgonjerm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2tgqmrjqv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2zegdwthf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2shjzmuif.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ktuaojqw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2krbwwior.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2efzpnvsg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yemmddbo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fciqomoe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2aqqhayok.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2espsgsxq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvzmyare.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jnfczjve.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ymhecftm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gondmzoe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tawgwpwd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ghfbvuar.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2yxfjaejm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2znnpdqgl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvxikgnp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oxpinvna.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2obimqbhk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zpaurydg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlnksayy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2psjucdqx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2kzlhodie.html


<!-- 参考信息 -->