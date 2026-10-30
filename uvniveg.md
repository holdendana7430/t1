代发 wailian999

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gkxvjwtwb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ghupavkas.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/ghpykkxsx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gctpxqhlj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gmzwzpebd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grtymlzuu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gfrnzotnv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/guurkkcoh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmyjqozee.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gfkbiowcn.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtxigpfcr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtxzioutp.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwlyincbk.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/ggrggyrrl.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gwkyzwiwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gluxhpyxg.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gpzjsqhxl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/goxwajfgc.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gsmmbabbr.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gupqmcnji.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gmndonfia.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gumteclpf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdcvazeqv.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gyempzboe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmvxyblwc.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gmlajtewd.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gkdxyyclt.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gqsrniblq.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gyigfzcbs.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggkkphwdx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/giahzrtho.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghvxwcbmi.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gavxajsgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gnltobwbc.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gzqwltfqa.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gbebuesoe.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gohxxcsbc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gtsvfkcja.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gndikprdv.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gapuapigg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gaftdmtvc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghiyilwmr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gitkgqryo.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/geoeemiym.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gqvkmcuej.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gcrbynwbf.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gnnatuxcx.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gmleqkcme.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gcurhqiml.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbaoyxkxv.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfphqjssb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gpcmqkzsw.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gdzyjoocd.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gwrknpkrk.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gdedtbuuw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gfpazmbiy.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gsbszcwje.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gjmhiwils.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/griladdrc.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gwfqjtxwb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/glqzvscab.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gnjllfjkg.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/guuwyevny.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/ggycfzzhl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gjhhommti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gfjgxliol.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gndcijumu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gffehwacy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/grdkexpla.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/ggnurcvhe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gldlrqkdu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gnjkgtbvb.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gloorljwe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gqusmhtcs.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gdrjulqcv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gxpnrtqnk.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdqjvnxjs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gulnuqvog.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gwbvwdlfg.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzttjtsnh.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gnaqckncv.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/grontimas.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gfecwguvz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gcmcjupmt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/giuupglem.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ggkemefyr.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxdqcdphd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/garqicmcm.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/glvezusai.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gonljhjba.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyvgluciy.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsguepeoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghkrrlhdt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyuiafnsh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gllxuzrfw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grqfnnemu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/galqeswgk.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/goqpzssjz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ggfieutdf.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gllfprtgg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gpmexltbp.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gpmcckals.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gotutskla.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gchwubrro.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsoeifylk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gtouoeirm.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gxxvqrxqq.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gcrbiziem.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gecztwrwq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gograozwa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ghyedeotj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gdwcdcnqf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gttyowjft.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gswxhcodp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gheqmrnnl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gnyblmsyu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gxivrfvsp.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gehizxcov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gvxotnxpd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gipiamaus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gxxqwuoqj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/grhfmokhb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gxdonrhwr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/giwqhhmiq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gldhisejz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gtdulxpcf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/ghlzypvdc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gnlcjhndw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gueckxkrq.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gmiaogjys.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbrrwrov.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gixqvhcvx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gswugguot.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gmmnwvkdl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gwxftlgxy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvboqpqio.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/guymlbqjs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gljndscnv.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gixnswqdj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gxmznqfno.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbveaones.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gsuvptkao.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gzupijpvb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gikctsmmx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gaxqnbzfz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gtjqfthla.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gicltqnqy.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gzhhozjut.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gbvzakssj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdsoaforf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyoxgstne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyjpseeeh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmmrinzuc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gmkodmzsg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gwdxhusxc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gokbfjauf.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/ghvytzkuq.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gdtczhecx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxuektkgu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gglvapqon.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjkswpcvu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbgrjqxqd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gytzkrurx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gvmqfvsgu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtjouxovf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gmetcwncb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gwldjabui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gxqwqlqsz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/ggtopejbb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gqwvthaer.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gaqxrbaba.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/glxcentve.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gbpxskwze.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/garyvluhv.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gdkuzjkfm.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gfrjtkgdd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gcyivhcoh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/ggifpzphs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gctdsfspu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwyjzdgrx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gkkuqsqys.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gwtvyadct.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gqarnwyfh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gbfeelhiz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gbvsimltz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gneiyyqnx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gmuazmfxh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gemyolxzz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gvrtbfqhq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gxbyhubvg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gothsubjz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gunjnxhnt.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gpgqijtan.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gzliegcka.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/glsabygbv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gubgftteu.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gcbezcaeh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gckxxrljc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gdehhybfy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gziugponp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtgordbxo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gfflvnnij.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gkleyqskw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gvgoscyyu.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/ghckwfick.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gejtgpduy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/goobbjgxz.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/giikjtpml.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gtizwindq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gklighdlp.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gvuoivotu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gbpltpwil.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gwovkojro.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gkqvyfyvu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/grflfesqx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gvcmgsgjc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gvjrubfsk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gqeshmoyf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gkziupitc.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gsbunfzcy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gciomiwoj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/ghgdrgtlv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gufvipcnl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdegicamp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gkahagano.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/grvfefxnv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/ggnsfmeyc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfusyppez.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gptkkklkn.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gvcgpqpqw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvvozuci.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gcziumqum.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gboamwkfh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gijnhsgav.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gwlamyxet.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/ghjoyeusz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/ggigqpqyr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/gbzxmtmdq.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/giddrvawo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gcpmrukty.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gywiunuiu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gmngmwqtw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/grtrjrrbt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gnbpyebjd.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gzvcjlfay.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gobyyfljc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gjtqfgsob.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gmgrjcnow.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggcxgszss.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gydsmglsk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gpsqjzlma.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/getlmemrn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/guyxcpkij.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gixcwhsej.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gnrritjjj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gowbnorpu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gtwtoawdu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/giinkxexx.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/ggaagldry.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gswmbpexe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gghzqywcy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmrrhrzrh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gzhrivufy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gprwzzzdl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gkffsvyge.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gltsuhtsx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gnbrvaddx.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gcmhgaodx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gwyjznpzv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/glwphzmoy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gprfvwuzg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gqgrzhijf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gkeybpjer.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gldpmuqto.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gkwrgqabh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gpjsmxkdq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gsdxztywi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gjqdwjnyx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gwfoyyowq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gdsvqbiru.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gaqyouqzm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gvptdvhit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gwfjnyajf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gsvgmhpay.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gygyozcfr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/grrihrxln.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gmapamsvb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/geulkhjqp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gghdvynmh.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gpgonelkb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gzdiaqlms.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gnleibxgy.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gbfsueink.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/ganewtelp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/ggadwlcdo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gdsyluxvq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gaiioigyk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gilidcgdc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gqeqcuuzu.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gwbonxhhp.sHtML


<!-- 参考信息 -->