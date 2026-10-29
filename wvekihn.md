代发 wailian999

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gqpfbwjgb.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxhoamyfq.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gyrocogge.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gnczipehk.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gozkipamc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gxrlquhib.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gijgomsoy.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnpnapzss.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gmmwofhjs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/grzddxjzv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzlbhsnve.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gztcdlmdh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gyklkvaer.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gecrxyrpq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gtindivus.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/grnryfnsn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtscykyez.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gahixflrs.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gzgfixfkh.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ggeukwujg.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gzdbwnlds.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gketsqjgn.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gbzwjnpsj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gcqsmmsyu.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/ghsfcfnjh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gegfntbfv.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gjcbavhby.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gksyxdoyj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpuljfkgo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gyjvqarqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxxmkvixt.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtqrvfyil.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gkxhowcbl.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/glqeisivm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/grzmhqzkp.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gybbmdkql.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gvwjpkhiu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfqeasvkm.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdaynegsk.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjahgjztw.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gazalydvn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gbqjlmzca.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/ginrjitxk.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/grlmujdwa.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmikmkfhm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gscouujjx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkjebvtvt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcsazbmy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gikjectfe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdlnlumll.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ggxbyadcl.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gxwizhxxv.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gjtwzarwb.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/glqlmhmxi.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gtwjavzed.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gwotmtwzi.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gldenozlx.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gpsmmhwww.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ghyzbavfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gnvyshzsj.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gqkjsaqfp.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gisqplttn.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/goeqhhylf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gztqaqxlg.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gizsuugrj.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gemadadsu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gykgpncny.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gvgevsyri.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gnfkxvmtw.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/ggsdcgnqg.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gurrievyp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gdomfrvjn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gezcrprcr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gzwujbbdj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gtbtniygd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/guijkling.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gmvjjlcem.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gcxbpycgx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gnrwbsbty.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gfkiflvur.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gzamikuty.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gnxowhmvt.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gjdowkqnl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gsujcdfek.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ggezyheej.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gszfoppzz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gmxjtrkss.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gddxbownm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gxihiqlkx.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gnliooxen.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gpqykgxuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmziymf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gjmjtzcxi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gcaqflfzp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gshtuqoik.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqqjchgyj.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gtciohbyl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gunzrcnke.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gxlfhukww.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gjekiwvbm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbzhvnrqi.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjjgnljaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gibqtswps.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnjcinfmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gumkqsgtc.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/giwncazfb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gtlbpfzsc.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gjczbxqyn.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gysxnxspe.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/goerxkjog.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ganxtnhbf.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzbexkngc.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggmmqvevx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gfwfsllxh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gsufkdzty.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gatchxbcu.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gelsvzsya.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gexrrnrln.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gpcwqtygs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gegoreibw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/grfhrybfa.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gdzzxmjze.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gkmrdhabe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gcdrkeemr.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/guykysqod.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gwsfyowcy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/grsmikfah.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gslurhoxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gjxjstqea.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gfcdnxuhw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gsjbsvulz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gjuogeqfu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gnkidbzlt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/glizggahn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gqnvyaumx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gremvgkqj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gckbcxtci.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdmkszzkx.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/grteuzqrt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gpoequinv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gmmwgkprv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gppfufhbo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gzikpgxbq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkwjpsbnd.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gaxjjgnqc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwnjjlnby.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/giemymwqt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gdkddyouo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gzmsnxmqe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gfidiuokr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gouvjbysj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/getpjvpvv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gjxveceyh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gflfmtbow.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gcchzdjnd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/goylnxljp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gtgivqflf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/goqntcjve.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjnzfqetl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggveepcxu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzgdfwxyw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gbpgmpqqu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gnhrsewic.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnctxuabn.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gljuvketh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gccuoyhxj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gljdbvhte.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxwdpbtux.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwlhrnplh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmcnqtqvh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gyghvtiup.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gdlbuoydn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmjufvicf.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gtaixueyf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/getijgcyq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gotfwsvvi.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gtxhjpndj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gldcayhwt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gmwzngudm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gadnwblwq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gwavuzuqf.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gxlvzllfj.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gwlwsfjrs.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gnwbdbaei.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/grmkbrwsz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gwoupqvno.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyotxeffg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gyfpvrjcl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gixesqbtm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gytooqqwu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gazkagohq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gbzcpgdwa.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/guvypdxko.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gybxfvdby.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/grprftqyb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gytxqkslt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gwvjuhodp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/guddtsari.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/ghyoltzut.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gzfcxrynk.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gjtwgzagg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gpbcelcvb.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfpgfnehd.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gljlheqzz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gjntpfbdz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gcmudfsmn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gmfdyqfoo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/guodywgmh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbbqhphmj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gqochjpbc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gdzhsalri.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/giwrvhmfs.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gvtrxmqxg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxzgafn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gfemxjcbo.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gpvktoaxw.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gviyqceni.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gryslqnpl.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gdqqefykt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/guodjtrrx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gtfvylgkb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gxehfleuo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gcitaegku.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gnnzqlkbp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/ggritujws.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gcawpcqkn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/goktogwqi.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gxgurjdzk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gvrikbbno.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gjzgrlmsv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/glwzdxgoy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gvhrhrajl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/grnhaqcuy.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gjslmxmvl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gmzqlugqv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvjokbuxw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbcdvnnvk.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbpqmlrtj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkvqaumux.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/ggozkdwhe.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/grirquhox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grqnsofmh.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmhfjocdi.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/grdwlrfnh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gebvgtics.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gyahhonlj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gqwxmsjny.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gxmyoutfw.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gqfrcafgb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gpkfkdpcz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gzatuxmfm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/glnndyzcw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gtsjdbswo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gqkimomxe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gpneqedyi.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gqhilnhvr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggiyyhtdu.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gdhocpfvv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/giuhkdyhn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcugfrqik.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gekdiwdzp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gkgjeycur.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/grhvcftdd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/guycdgztp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gpdkhtggz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/garaeaozc.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gpckznvlm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gylwpwpkg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gylbjlqgn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gcptiddqy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gdebxksmy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gqxzkrtpc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gxryegqtb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gvoapshjc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/glpsgrnzr.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gdbgrdtoc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gachdlptx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwcuxfwmm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gjdbjrgub.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gfimgqgsm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/ghmkgdfcu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gytoywlfq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gjwrkngww.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gfhmtqyxu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gewpganup.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gkjkcevex.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gfvzmnlje.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/ggnaeqnbl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gaeowovja.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gojuxwbfm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/glrywhbcp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/glocdbnzn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/giojqtnts.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gxghzjvxf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/ghdnbhxqn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gfxlholcp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/gkabtictb.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/ghlggjpjp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gdjggakvh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/ghauwiikp.sHtML


<!-- 参考信息 -->