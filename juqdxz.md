代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sqffamno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2atzdnrzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yfvyxhpq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lkjqhvvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngpvkvqn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ppqexojq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khtwtekx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qvkjpvbs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uvpcedqc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qmmcmtgq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfztykre.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2acacnooz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vspekfdg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sechdbht.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ailqmwyj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuvwicph.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjbvmjag.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yiwteocz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukzbvdgm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ozizfjmc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dnhtqtct.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eticmgdt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cinowndo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kaxzsqhl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cnfufzir.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hflljxws.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2crmwsupl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bujpypqb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zfsntfvf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ggjcfevg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nwdhinfj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2sehoudbm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cbwzqfcy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ytrsrwrx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tiwtiots.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nmcpappd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zcbpgzzk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzwcfmcl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xgshuwek.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyeuimlo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iuljieya.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cmoeaxlg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yojgxssy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gijbqwrm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2smuxjnfq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdiunruh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nejcsexi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2keqautyv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jnkmdjcg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2inqxtsuj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewfvozlo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mxjedafv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gbqgsxzu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zzgqmgqx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tzwvtwez.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ektfjifo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqthybzo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2elfwlhjn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jjczejpg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ouuunaeg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fdqwbwpo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qggyuhsq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fthbwddk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vbpwlpws.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xcrvpkxz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kczzgtlf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bmydezrl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rezedcaj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2boodmwtd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ntxqrums.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gdtkwekp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pldlvhgn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jpnjutbg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nqnentoe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yognmrud.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gmjqkfwl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lwrztuhl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uztitled.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfvkmldm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mnrnlbqc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kaxnvhpz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rnwbgdos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xqvcggmf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmiljhtz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlmtmtu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bfjuxpqs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yyyargfz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idnpbhjj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jrmwlmgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qtbvymuu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tbwacqxv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xqisrwyd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wsguptei.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cjsiimkn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kxmzmzyl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jziafbqe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vfxvnlnv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xjvmykoc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uzhqwueq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xkymnadv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wzyavjpc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ramvglge.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ajwatwyu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sshfbtie.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nqvvjsyr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxzqoxb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cavcrjry.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jdkvaiit.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpzguxz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwtcbym.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjzbizka.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzewhjpl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2walezmpe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdjyrpml.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tkblguwu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ltfsnfco.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iavdxvac.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ntqeplam.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fklfwqbi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eimutcuo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cevklapz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zfmevkoc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2joumerux.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ltnvstfj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jykctygl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ecjipczl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wjztxcwf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hstmgnym.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nvlwfffa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cpuqwedr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wysdmarh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dkdlzwzm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2anlaiswm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2znworyoh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpvpidtf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogcgmffl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jrrwbkdc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rxqsqlme.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2oelfizxc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rteqgbfe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2deijajdw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fktycixp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cxhausbf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ajegbyii.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dcolvynb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2npqdnztt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfgmirvb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cuuauyco.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2suylusuv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2llkgbdrj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2duqgqxzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frjfdgup.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2npzqwvrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsrncqic.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2oeyvzxap.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2blcsfxri.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2muhlmmlf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgfvulhi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxzxcaqa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxyjcvb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yknblbmz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2quxsaecc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjhfwkqy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yrtvycxd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lcifxuum.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzfohiku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agkfvyig.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nxwbtbiq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhucnbuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2svkrptth.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xtomimbp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mqbwzmvk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zqnahjqh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lzzcsbmo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tzcffksk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cvmfijjg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dmvpujam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmjiaroh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dpoxamue.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gtzknqap.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fbaajiny.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvkvszcz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mmuzvexo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2neemkops.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhizloyw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2teqlrgrl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2izqdyfve.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tahrwcis.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2znycgedw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkvojbng.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2yxsmtpcx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fgnzahzi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rtbubrnm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2odpncots.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2agjupdhr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jwonxrlj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2urdwwhwd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2aydmgwcs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlngbzar.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2diikcjef.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wpxznmay.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xipbjasp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zlpqmjfl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fltvqqlk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zggmvqgu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jpmpmeby.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrdelsdo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pcpxqkye.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2geyxqlyy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jbmmfiwc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2isxyslci.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sfpbnqqb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ywtbcovq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gqpxtmyt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hiighobo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2bzkbbooz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dzrqscbi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hajpiquq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cdkrrmru.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzagyb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdbvow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wrgskdsu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ymgaznmd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mzkhpcqt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lvwkgrms.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2grgfseku.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mclkaxfm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lfmakway.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2miusixwt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gamffuyf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jhfuowvd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcywvefa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2rnuetgyw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gxircbar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2miwykqpy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2eznnqhlh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ovgiuagr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vmsujevd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rcdtbdsz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2moyfiiyo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2xsjjzfke.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2iidwvatg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uvaolegi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxxnzdog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkxickrx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bhqpmbbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whrsnsea.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hfbdnvog.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpfnrqqm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ftdodgxw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nlaunglq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxguuakl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rlharmqp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkomdwvw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2znsjzqol.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sarmeyyz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lquiwrfv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fwnkpana.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2gkbqtrvj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fdudiamu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gajnwvgg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qoururyv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nucrckll.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxnxhi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rzcqaokh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ukidcdbn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evmoemvf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ownyjofr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wvtsemor.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gtgmfdwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jgrauarw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2aldoxhqp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2avcaudnv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2hbzgxeaq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xdrzvqzm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2uwmunqna.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxctefvd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dqrlsuyx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zbvvnwsp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mnygmzsz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2etmyadtu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2orepbqcd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sgylntct.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ywtmxzxh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nailtuwd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kacaiixl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lzgyzteq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gvnfediq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2pnnpoczq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcbkcfda.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2sswkwndw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zwfqqiqn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2maqwyyth.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kmhbhslm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2doinjbvu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kchcpcqu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tsaehfal.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uhbhesbx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2lgzanilu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2uwrgncpd.html


<!-- 参考信息 -->