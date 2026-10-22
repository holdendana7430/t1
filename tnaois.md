代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjdzhtu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fkbdeoom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fwpxglqh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wdhkyaua.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wvkwphzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ozgccvxg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lkldvisa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uilqiwzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdhcleyu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rimdsruv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suuxfnvx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2elmvwjmx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nwldiuic.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jodsucpi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pftnwrls.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxntzygt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnqtvokl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hjcpejvy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sknthiwg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbuflaoq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vyalpfsp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2habgvoxz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wexfkaaa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgqsvurs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2capvjswb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qpmlwrjt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzsovyh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2przgldeu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfghglwy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mwvhpeba.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pdghufgb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gxvmcric.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qbgzkcqy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xwxionwx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ymirsbli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qiawbcwx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fgeleomn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltsjkfqj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mfmovxzu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nmkbxfyo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvckduku.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wwarejwq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kzdoqggq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wykmxvzx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xrhozvyi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tksgclyi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2npqoehxx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wfjaulfh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gstwybmf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2obvpjebg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyjaywaf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xlzifvvv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyvaxfro.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bwcaxoev.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2svwzuqey.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkiylzxy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qyrecyui.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cdplnvlo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzkecbfh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qmeqpxvg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhzvvzdl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aeqmcadk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2senbiyet.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uymyiykq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xamotwfr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mcrtgoij.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fzmmdqyn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qujubxme.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqhbtl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zydaroyd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gqvbfvdv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rvxcwxti.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2opsiyewu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uyskmgzv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cedggfah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gvgmvxwa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qhbkwkbg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2crzjwavi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvbqiyjt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oxljaabr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hmbobamh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jybctkmz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfyloagn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qdoqnofi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jisrgzuu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2spwabgvm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gxptejcs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lwjubuyx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztzzbvzs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2omjtiuye.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2amneqmch.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtcvvxty.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bjlbsgod.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2svpyaytl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cjvnymwc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xjrxdejj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2embmmsyd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2eubetxdq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ozdthbok.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lwaxlcvi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uwatwcxr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2egthnqsk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jjavmmhi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vqygelpe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qdbmnmkm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbkbkhyp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kgkjtuxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zdpazwex.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yrswwdgl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cezyimjx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lpavkcbw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uxofxwps.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lqxvfizf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uekxdzvq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmmzrhh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jojipsmz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jqxcpzux.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jiagkjxp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gtsazaqw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hecjnzdn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jhtbqcim.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vxueaeyf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xovtwfqf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gsvyuqbh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewhohoad.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2anhrdxxn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2joitwrgu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rfntiaii.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2azsombgg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mzdghpkp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jlpuezvi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qjaplvpz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mnoctvit.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2udwbpwjf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2orqfhwtg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gkerngsf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rizllcxg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xhenveog.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pwcdqobl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2aqqqmkvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kyzxppli.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jvbfkrpn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2aojrgtnm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qlywucaf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gcogswwp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2azphxhpg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gnwotpyb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cnsmkvbe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xeeojqoi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2imnsktdn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymhgtsur.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fviaswij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uukfxbyr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ioakekzz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hmxbndkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvwttkpk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oiourtcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptmubgnj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tkvbrbvt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ffcweiga.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2myuaishw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlskyvcz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2srndnagv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cfzipwom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wvitmkxe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xzzafchi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pexnyour.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rscnwibb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2bnbbdtqb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2euqympkp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtkicmij.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crdirbdv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeccyjll.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xgurndel.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vguvswil.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2degnufam.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lswflhvx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yjsuldrz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pmhilrjd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uzjimlmg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rrsqpmah.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2arrvpebp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xfebsmnp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2iapzjxii.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gfhycmxl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rhxdruqz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vtuyoanz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2krtgjvhn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gafbvgnq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2megcdlxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ufasfpky.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tiadzgzn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ihemszva.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pvumsjjm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvjuhqyq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qewenblj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zgpngddz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzsvoyak.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieqzgoyf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2haamrysy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cbuwhojr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xfzgevnu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wohcwfgd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2odzrzhtk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lsseqhwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bwxigmsf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fbeivimz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dtupzhtj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xutzsadc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2taosizcx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ttxpwjro.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dvtubomo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2oawjzojp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yraoxjjb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gdmarfne.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ecfntpit.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gzwwwicb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vavmqhsk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cxyuzvrr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tcxrxfsg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2btssyyek.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mcuhtnbv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ilmamouo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2avbvjluo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2pifdalrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kckqxiwa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hheimwko.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ydwwvpne.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jzsoatyf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2cabdsfji.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ljtbiqus.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fxsktzyg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ztffbtxd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bwsbskco.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvzghoc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvanwnkj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ieuefsfs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkpubfn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2suoedfnz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ualbjldx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2peyqthez.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2iggpjofu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wlhblxqi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zgmacmbt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2klckuiqz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tgorazva.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2egtwuwrf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bycbeict.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uigaxnpo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2exapnrms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdjjhqrt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wuskmurq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hqqwfrtc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ehlitgwr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdvxycz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2chfueflk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fqyvzxdg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtrgwqf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dvqfjtkz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2knxjygwf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kvpdullh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xaosjsfg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fvugarrq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pnvablbe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sozazkqa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2exlvzyun.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqgehwv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2txeicqnw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xwvwtwli.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2iubuitpp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cnvonjva.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kebcswqp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fujrkgjt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hhamsmpy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvcaqyr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2nfootbsa.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2cjbrvrcl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2blnpwpar.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fzpzlqsk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2slwrixly.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqyuhnzw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mjekeypr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ufwncjse.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sglkcjoa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dfgdknqu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2bzumflgu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gesjeijb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xnvwdazm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ekjmdlqf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pdbphcim.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxcamjpy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jaolefhb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ifphsczb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zavejbyt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjbnoki.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2agknqewb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2niqqgohp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ljqttgme.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2nwmmyuut.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qyaxpbbt.html


<!-- 参考信息 -->