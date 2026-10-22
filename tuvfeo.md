代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rxylwabz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cndpbhoq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2catyjuvc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2louzuklo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lkrprwwa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2stdxhhst.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qivpoeyq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgnqzoyz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hktlrmzt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rnslyhrz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhqfkxtm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oymdyusp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fvssotsk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chbzrmyr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2slottnxl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qicvlvqd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2toogrcrq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qjaqwcpp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kupuhkzj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2olrkuuvv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pltxpior.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hxihenca.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2stxcifgs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ituoxmtx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yibnqdvc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdwnzzmt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zlpeuonq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wwlbwapm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2payuylat.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywfdevrv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzqhczlb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbeqyuvk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2muxnikqy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wdusnwem.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ormszcwb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tkcnweug.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iaeidrpo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2asxtwphd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiaziele.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovdbnpxn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wlhdjmpd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qcdeuusi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqqebqqj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zpbhjiys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pvubelis.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zntcydak.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkmetotz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahwwagrt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yabenixh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zsxxwklf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jrmdkzhf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cowaasgk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cexsgmrr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2duuxghpb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tdeglftf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2foaobafe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akdlwosx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zrhkxgto.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnvroxjb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mzghloac.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uenfczrd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dufjqvje.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nitxntuo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fbekwzqb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dquzezgg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqmfflyq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bmtfxtxz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxpbgvyi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mryfkvgl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gtcourlv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dshaldkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jtvuywnx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ozhysond.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gonvyjwl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2evhcgkrd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uikfyrox.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ifvabeps.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aicfavmk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kvqrgqid.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fseigdku.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2aznxzdlb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tiweiqhx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2idipkqmv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2flibuiaq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ymllssna.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iwkewmoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xzdbnarf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2phgkjuvg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xhpcjmar.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uwpbtmhs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fgfbyira.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kutgaafg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2aehbdnds.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xarcrmlk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqvutduf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2khypjgma.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hcmmibdp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2doqdriao.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zuzdhybz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ysrrjlpd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ovgkadqp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gjlpaehx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiggvcnt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxlhzhoc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cvsvmujv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gbgmjxbb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fdqpuulf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rjbijixe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rqeviooa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iljdhgsg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kmeodzwm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lilvdfkk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yilvwzkl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2thufiwmd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbadgme.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fyotymjb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2syihnroi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qeqzjqqa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2avujfmto.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tsomgdmv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2aijrvhgz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbvidosq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrcnuki.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hrdkfhau.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2abjmgttl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fnkfnccs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2petnjwwu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zwqxkgft.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qebdrobp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxeindzr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vixcncwj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mlcsmkaw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lywjvgmy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tqldwzfd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sluyayes.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kkofyqxe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bwiusxei.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhpphmr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zprhdmcp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hohrsoie.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uxoimtcw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kigednfv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wzuhusik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwpcbust.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2udzpuyyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggyaaakf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kqgyidyu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2eslnacog.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjurwyvg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwymxvqp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqluedyy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jovfrdzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fbtrqiqz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2shwclcjh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mcbyndgc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2grgauyzu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2frqbfcxu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quiqicag.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2olztqlcy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qounnwty.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pnxiluxa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2owlpuosq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jypswqcc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyqfaokx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jjxcoqab.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cekqsaob.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zmylcggr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sygnulvd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cgbndmxq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vdofpgfy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtzygrp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vuwekqrf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gtjsvoup.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fkowdfvb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2djlvxbll.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouhzmoio.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jdshaeuu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2virjevlc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zvzzsimk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2otirpxfy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jwmkyfdz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fxbepaqj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lrqzqity.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2cdxyitwf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jgpgthoc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2brspkpgx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2alnkaaip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mhvwikdu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2racrcnzh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2caazurib.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wlbzsgxp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2eichpmrq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ryquwhsj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jbelhcpk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhqtqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wxobncnw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2fpesluzt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kyyfdyfp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2akzkdynd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pqcyzbhd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kcnerlxv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2bgojvfst.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pcocrkbb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nyrwdwzy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozwhdyml.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kraojdyk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2htrwdsrw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aucoafje.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jncpvbrh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qeijvzzp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2idmuuxim.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2smikpjki.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dshezfrj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pjpzctcv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcagwj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xkgrivfe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gpqzcgqo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2svdvfnpx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2iqcywlbq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bhvpwqdf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mwtvhaws.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zfjttgjo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bgjuorox.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bwvjnddt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hkglddam.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xwtkjsbb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qpzmysvb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sximlqay.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2iqzllcwk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2psjmegow.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2axdcikmo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pznrscht.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fwdimidl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pqzeegbe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cgblqzto.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ojlihnjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xddapcup.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2scswxhma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrewfuva.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qvtlmbld.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2stkeyusa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvzurmgl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwlscdh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jcwamzxr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2utakzmas.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2desmxtzw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvdxevc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bauhgoam.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eiphwzym.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ktnpcvxf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qvqrhudv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wmttysje.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2csbebnem.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2abqrcuoe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cwrqbvnx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lxwnldnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2duxtgzsf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2deivuiby.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ekudkorn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xctssbhk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jxdgvvbi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2orcqhqep.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2waibqsfe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fdcnqsiv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2vkjaotoh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yklnpgqh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2snicepog.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dyuqncdu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2emjbrlsg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qndydjnk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cuiubbzt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lrynjyvu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ndmjpjri.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2obtuvheh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xjoupatf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sibiaais.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lvywwbtb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xkidsfrq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bjfyjwdg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tltexmkb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xfdvagfq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngoqiqct.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2akvenpfu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xoxycafm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gtcvtgay.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uouilbxc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2caiqxewf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mylnhpzg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2npnilvxy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2adhbmuoo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ginnqjyu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jwcpwsqk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ptyxdvwo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jljbeuoh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nznvvsjj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mhscvcxh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pfgsibzy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2fomikfbb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vygiitmn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2esujjoon.html


<!-- 参考信息 -->