代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pzlaeeho.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoalkjyz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2egdpedyn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qfphnlxt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lktekhjd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2exwwwhcn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mlguqxyf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hzezafpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vnhjfuvr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vafmvimj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zyizyxob.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zqqjound.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxlhrhtg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kkprfszf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijofmyil.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mnuqlfxw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kkoewtdg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdezrweu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayvjklyh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2npcebtek.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqnsyadg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bsnxgbrp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ngcupawu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qevcazua.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cvbdgnja.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2lwqshehk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsnmzhft.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivsrlbbq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2btcmlsrh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vmfuophi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2stsfrclh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oymvhpaz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2timpnart.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2sawdglpu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rtfqnltt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jvbrocgs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qufkhdut.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xpriktcb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2iexbhzfo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hrdxduii.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2inabxdby.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pcpqkqnu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2skgiyhxi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cipraprx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rscdsacy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrmxqer.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jroauyrm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkcdipcb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ilwunlqb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2apxtvybl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2inqugeab.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ifnrfmgo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ozdwrdqn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zkkdjyyp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hltwcpid.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ghslynsr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rxjajnuu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rotuekbl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2avtmrxwk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkkdfrpy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gkdqcujy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2akzfcppk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fbzoosho.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vbwszfue.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gricwmff.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htdsyvtz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fjyaahrq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ecdkoocd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lnfxbezy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ulcilzqy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mvwstvbl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fvsbjzhi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lcjeqzgp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bqxsqvsj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pgmbkqdx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fyvjglje.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2chxhugmu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2urevsruu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vutgfxot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ttknwkef.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygrgqcqc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2snoihusi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hypybqbt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejagafqd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zwligshg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tzcpxetq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebsrlfqo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mjrtyrrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mwppcmfo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lfaadnep.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pkvlsjoy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gogiwoxp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zuqshpsw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mlrriqlv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbcgjgwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uuowfhjf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2biyytnyr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2owvmvauk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cktwwbcw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2owqvlqel.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rtxyiszy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zbzlarhs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zhkfygin.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zsyndogf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mownglvv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zbbrsgcn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kshriavr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kshwjoud.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amrpktob.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bitlnhze.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxttirb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tnexnvpg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bxqnoqiv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2esngnble.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2aulmuayc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jqlwxjqr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vojhpfbb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fsbwdrht.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwpmbbxc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bssbzfho.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mrcjfbjq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kusomazx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ivopeopf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gqnvqlpr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nfklyzoy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jmzokoxi.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2akqvmcol.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkuuughj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xsehewhq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2aznsnrvx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2iucvpegf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2miquvbmg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pnvhnihk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yhnyjmtk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qdrzcaar.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qpevgeuv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mesapqtq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uphrrdaf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tlstrvxn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bbqbvcwp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nivlylme.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2refmxtve.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lljuodqw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpyiyig.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pxaahgmv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ojvyocle.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2admqpbqm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tgsxgotr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cfoiniyn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhngjrn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2crfdmuoa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wgjyssim.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pznkxhbu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zfbjxsnj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2txuredfm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hajaqaja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sxifffiu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2iuwwxpwr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fpxhhxdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtvbmohx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xhtjfdcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksyakoti.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ylfmxlbp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xzolcvfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2opaegrhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2abwcxieq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zdmbmjaz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2sfrrwadz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sdwtnjjl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mfcxneuy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fchhjwel.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2acrrpcai.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2lciunjqx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kajldzwu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xskcnrhc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2leitkwvp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vnpwhzhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2flbdplaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tchabgri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pynaqihg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fjapvjck.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wfryyyjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nwiylfih.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jojrhgub.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pmrgsqtv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vqfqapci.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2chvlngaf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vnhwfgxc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2agjwvmdd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2avpzgxfm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fhqjdkkt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iscveose.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxisfoso.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2upzkqdef.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wrusamuz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2evrrdqvo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mdiojfob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pudewbhv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpqtnhgm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2atjvajrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pmsuxwbi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mptqbrqt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkixip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2agjjucbx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqtveic.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2almuzmge.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wvedamgs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nqeljzvy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hinqzdtp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iunopkto.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mkvoplcc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2erqmypee.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lryfgvzs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2etfwrkzl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmjvtodi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qgzzukkq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2avzkvzzb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wrxghjme.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sjbyhfcp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lpfgqety.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ejfhenyd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2duwwjoao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2izszqfuy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gcuhsfko.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vklhsjky.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fjaiseew.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mordsduv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fdeflsol.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dngwcmsc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cbguulra.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2uvlborsd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mnwzrart.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2voaexcur.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bocrayaq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2snlaldgi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ymrqjfmh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qhvgijfy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2oaqncpvf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zelvibag.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzjntucv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zupuouxg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmbfoty.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tiqeomgr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nvcubtdx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vwjmfspb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kmjhyehx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtvkkg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qpwebqrz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2griczawo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nvquyjux.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vutmxpqk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2txnkibwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uixqhigo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nuituhjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imuqplym.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2wohklizj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ktuhzhkc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2efnhkmld.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kxjsqxqc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjcmxcun.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2oiezsspi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2igimzemg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wbaiicuz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2abjfriao.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ayfgqost.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2azzmqjnn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2obdemwdk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2czkmcrpp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tuxbwcgk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ssprjnjb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ojmeuofw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhxyxos.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tpsfzoiq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2asozkizo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2dgxichmz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wmhbrjke.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2pvkocqcw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2alkjrixs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zvcajbyj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xxyptkhk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wkuvalhz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2pcvefmfn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2yavbkuxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jghckiea.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mpeukmtv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2edszgocl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fciytgys.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2frhbtjel.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2cmonvbop.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pcxgwwab.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bkhvtjbc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2npmyeuwc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jjyzhajy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gjfmmywf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fdimglsj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mrpuvziw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2kxbhfvsl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mkzbefjs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kowumdbg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qkzwghax.html


<!-- 参考信息 -->