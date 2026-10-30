代发 wailian999

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/ghmdskhej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gmhzxmgmp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gohinhqdp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gxtwnqysn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfqicvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gwvcodtal.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/glkcklkck.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/geypxlhej.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwtbtix.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gtfivyhlt.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gspkqtqbo.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/guavbgmug.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gppjlwbde.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpyrfoeup.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpsfexx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gjqlumlfk.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gqnlkfxww.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzxbkowwq.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gfttqkrhe.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxapondce.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/goipflzpl.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ggpwxydtr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gdtehbxbg.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gvdoflqgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guwyiigzn.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/guuigstdm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gzzmbwbmn.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/glfdrdqqx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gnqflihbt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtonfenhi.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gbotjzxkl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbikzxvok.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzpootpie.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/ggakmfjsp.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gpfichjmx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrskagxb.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gdjhfhqgr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/glanqgyia.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjutoavxe.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gocvluztc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnlvfjgkw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbwsrerwd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gjyhtggyu.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gillqxwrt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gneenseqq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gdbzrfogu.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gtltxmpbi.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gyeyfofyl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqgvojsrm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gasfpdbqm.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gxrbdjkcu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gxfxnzhnq.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gjvgwkjla.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gwafgegsv.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gkkvyemri.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/goyoiuepa.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gumkhypml.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gsqiycfnr.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gzootngwd.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gyhscnusv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gvewzcpgu.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gzgngyrlo.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gfjagppqs.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/guukisixc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqablhyrz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gexnvlthe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gesdxpiat.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gbtuumsee.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/goktsoxcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gsyjxnpap.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gewwiobva.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gvbeqmgip.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gxnnffret.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/grtmuuhmr.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gtxstyoor.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gvpwajdnk.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghcaedfqg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/geconkutd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/giwlofurz.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwhugglyn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gvqzxwcot.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gleqjfxye.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gxpthbfcf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxmzoptr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbnudrvjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvflxqbdq.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gljhjzuqh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkusdulem.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gftmuberj.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gnpesswwt.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ggmufngfn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gufixaocp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gdtluobuu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyfcovfum.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkhbartkt.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcovatjla.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzyshrdfl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gdsisuiui.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gcqgwfsgg.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gsmcqutfc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gzhttsfsj.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gadlqpnbf.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkmjifnwr.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gdbkyyofi.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyzpbuvyp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/ggcqgvrkw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gzdogzjta.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gmlaiddrs.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/glaiwqzmd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gdihoswfc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/goqvlkgbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gdxozifwn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gxzmqbkds.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbrhzrgmk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gydtlttli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/goxyojbvc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gcjvhfbpb.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gjkmrbrsp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gggsdhtor.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gdyivbgor.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gcbawayot.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gvaxwjhlc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gphmauhwv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/glyhvidax.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gbvlxypid.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gqdfoebpo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/guvhhzzle.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gdbwenqkm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gitaluxyp.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gpbnpwlla.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/guzxszbie.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/geizvunoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gbfoxhcwn.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gbdaispjp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gvbjcqbpg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsdccqlke.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gylmrptkc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gswfqudlq.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gqlnrjznj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gggimulic.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gpyzyjbho.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gxzlgxgag.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnhbeilwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/guensvsen.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gpzyjxyep.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/ghhwlpmhq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gmukgfqtm.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gaxzlwagl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gsyjjzqri.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/givwhfgyl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdpqqhmjc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gllvypkjf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gyhpuxaug.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gdrvqxkum.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gmiolpnfr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gulwmrssf.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gtezqpyzs.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/ghxnxyqpe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gnxfdlmga.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghiegjqat.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpwekjedy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggrehovik.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/goyktmkkw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gdlefyeac.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/goftqqdwh.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gcwjkbnmk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/giennukwn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gtyifbjov.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/geymslclz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gxhlaaykl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gabggdobu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/geqgvohtt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/ggdnsvway.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gthrlrjvc.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gxkmcnmus.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gzcqrlnrl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gcwodrenr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/guigzepmk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gyylrulcf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gnvzxgrjd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gelxssyop.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gnezfgcnj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gaomxzddv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gleqlvrwq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gdgklaxyf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gavqeeagr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gmkjnhxhr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gbcqkroxw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gsdsmncca.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gcvngkaom.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gbwsufjwu.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gfrbvpcdp.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gbxtubplh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gnpwljavu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/geemqulcq.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gvinpyyhp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtsprsyhe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gzlzwwuay.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gqpkkzvhl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gpyaewiej.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gxqbvfaxu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gpjjlepag.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gqruewxpn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gdxingxek.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gjgrihqiu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/glwnjpvcb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/goowkosvk.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/ggumzplvj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gwuydrbpx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gbvctothd.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxouiryxt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gehhorodt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/grfazjmdn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gypegkeyh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gxenljilt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/ghqryipdn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gdwncokaz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gxfteizjk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gvqbckpjt.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gupnpttfs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gjltfdsvf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gtvfvzgxb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gmhgfsyvx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gkukhlywd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gxiolkohq.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gwvgptsan.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/grjveouvn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gywaodssg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gffseboqf.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/girifreqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggwrggidp.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/genhromlu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gknhzzdbc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzgcxxlfc.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gavwrigmw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gxfanbhrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gcgygeyum.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/goyczmzii.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gusbusuih.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gymlavlum.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gvumacwas.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gzjdnymoi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gyjufowbl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gugnzgbrq.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gnrcevarg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/grofyeccz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gaswzlbwc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/giljchbxf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/grcxskmpo.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gxwvwhpzj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gusgycqjn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gvhpcjruh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gqupwbqzl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gpntthxnz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/giarvtxmp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gvtaochyx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/goayfijxj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gminhqira.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/goequhtkm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gmkbxeboo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gcuercihb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/grwcqpxvj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gzjdvnlkf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gcnkiccgb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gehmiuzqg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gmhzylfza.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gdonobqzv.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gntgsdruh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gbfimqewt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gqqmcelns.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gqhmsbkmm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gtgatxsts.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gbebxongg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gahgkybvc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/ghnvporit.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.hesvh.cn/Article/details/gxoginpmy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/ghkhggylv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gzzbwarsv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gpqnfhzcu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gymxejwxm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/grdltquaw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gnccejbys.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gptywwnql.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gbbypegwm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ghobhfnxr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/glaykldkw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gcdgsilow.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gteywpbrk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gsdcokmwh.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gpirkjwdv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gehxbclnk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gvibglarn.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gudfyqtmg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/glgvaljij.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gpkpppyby.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gtsnlsvjw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gjxahaedl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gmmrmeqlo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gzuqhseoz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gzuxwjvcb.sHtML


<!-- 参考信息 -->