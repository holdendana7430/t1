代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mjmceatp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jnwmgxpj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ravbxdcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bwgjrlbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oypgplyn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tjldhstt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzgqmmwh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2okfwaafm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lvscckgf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pdpzdkpq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2suwwyyzs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jpnkgviw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqledriy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2revgzhmx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2guvnwgfd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfxezjge.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2eebahdzr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qdacqpqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zlxslptk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cgfcihbh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wceafeih.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxunkfxv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qvscyzux.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2onxvzlcb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byjgyhip.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hwuoslsf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ufxrrork.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qcxfldty.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kjwdhqak.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dvmjtofv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qknxqypk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2upplulpx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qlykkjko.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2apxplqni.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yztfgazj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yyrlrify.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkgxfewo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoliuzlm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2stpzrxoe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guxpmooe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gxydsrex.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kmvpojit.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eclzkglw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hhremewi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xbahlcrx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhafjjop.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eftgpubf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rilbmvgf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2popgqack.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2urwbzstz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qndcgwwq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qqzeizfo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zletlvze.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lrzeinez.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqydptcj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpurhnnq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bkrymhkt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxsoogs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qkocbdkh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqasqffi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2aeixiskf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dnezcnup.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2noolbvni.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sscwjfjo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngnaxkzq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wrryvrra.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nqnxcmfx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oyxmrafr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gbcxqzwf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sswacpuo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2emjdftim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vtnqnhyt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cozejspn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2egyiqyyz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvpmzisy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlhertxa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zfmnpzeb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wdbzoeop.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yyzuovsu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2usvfewaq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2brfjxqly.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hqdkezns.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bgkbgler.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2maxartfm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jleolncj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghhsfhyo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jprhuxvs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywceakdf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2reibdutp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qocerbrc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wghmrxup.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xhpzoyko.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pddkxkse.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2knqyygib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zgvnfepu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ptlrzlio.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcgcff.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qfbghbsz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ylimdheu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rjxdcjor.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnxlzvz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lyulzdye.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwcbjytz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fcmkxgnl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nfytxmcj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xnghfzus.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tsiphtox.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rpiketpo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uqagmyjy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfdgcybq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlkgtzgq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pynzlsnt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcqngwy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nyddvyrc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qiruueyc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikeqmjdt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrgqnge.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dfuvkcul.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nprsucuk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rtpxlwuh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fiqhzhgz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2srnapcrt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gtrphtgo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ugslreuc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fkxjpbyx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aynarfnn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kakfmyog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nwflvrlo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2btdofxio.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhxvduvv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsjwned.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zsyjglqc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wzflfkxz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ugogvsax.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkirfrvs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gahhgrnk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qhyqsupq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kvvpqdkw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ogzzfztf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2uvanmiga.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2txceegqe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2emetuqap.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zpvaehrq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yvmttwmh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ladewuom.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjrarqf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvxyphwb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fyozsipi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xmyocpul.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mztbwjdp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lsrmgdae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2havmepix.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ivmlrdyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ursadsnf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fmbetpos.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dyymgxps.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqonoaoc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ngwjenyh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2abkunkry.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxgywlns.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2txcweorx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zqpqseng.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ogobpxvl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2brgivwsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vfahnkab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2opftjkxk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2codfqoqi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbsmnuzx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpfmjrhg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yttjtlmh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2evhtjvey.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uhyaqsfk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2criramll.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kteootzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hgwovdrb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qvmktnrs.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cwlfoyrr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wmwrucyq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nrizuams.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wqwpqtbo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dnprnuqz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2iljivvlt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2thjtcrka.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iwtkwmtv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rfwkpdyb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2drrfjxod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2azvixgiy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fvituqnc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yvdasdrt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ynxpiatk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cdqkdzmi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ssalpnbk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uiwywuyn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yglhjftg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huxfruso.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjzdojff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2llikhafg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fchptpba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wnkzawab.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2pcikbffz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mbvtjlxi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gpjjvodk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pnhyqpad.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lbeddrph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lixjjhoy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hvnofldg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fxohgpqo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lrcrzkrs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cbrckfvy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nznktcgt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2isibmbtt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jjsiffkx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ycztwslm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zouzhliz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wwqmiuqj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nivianhp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zamwrqbk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jtxaflma.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2eaiwbiaw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ydkqfciv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ebrwxbvz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2birtomyn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nsyzksbi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vrzvzrja.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mhmrrpte.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hetvoilb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bgnemdnf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vwonfhvh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pdrivdfg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hbromhfy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xbqrkcqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ochsoyxa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pvdyzngd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ilicwoyk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mliqnfoc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2llgcjvub.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qltgbiyr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xdqgibtt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ewvsytug.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mqxifpmp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2wrihtndn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qwhcpzdq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2svfyhxjq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vbxzadro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxarkbzj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bnmnfhys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfqzndvf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qiirfnql.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2msitussi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2feaymmbk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ujepipdn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzvnumu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rtrljvcn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rdcpkqwo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2stycphaf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qerqlplx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cgpofejs.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2afdizysf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2oavfissn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2febyjiib.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tiubxqvq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nupbmily.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tcnasqzq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mshttlxi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qrauojvn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2zzlloufp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywuzypqu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tqjcxhut.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dcjhgdgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2goytlvmq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2flfqxocg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ymhqsegq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kyphhzjy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wqpqvfby.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oyfsnais.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qnfusrmc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjozyzw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hsqdyqsf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qhklcqzh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jptmddfp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2snfjqfem.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lonnhjuw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vjdxexnz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2asvwwbmb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2weefpaxy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2blsjfnlj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2noaslzwb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iilwkdgg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2htvkudwe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2baiqbbes.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2scyobvxn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2maaglypk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dzqkimpa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lupgrwsm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xmgsedwl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2poytrliq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mlarlcsz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sgpzlumi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xpbfnjih.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ljuovjxv.html


<!-- 参考信息 -->