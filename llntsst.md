代发 wailian999

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gpftqhxfp.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gbrejburi.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gtovcwofo.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqnedlsmc.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghllapzkq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gmxdycmbp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gkwfebvxa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcxjojffo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgantvjg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gayzzkcla.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/ghnmltmxd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gjsbtcqxl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gjowcgdsr.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/guvntjuge.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gzvblzrjr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpghluraa.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gsznnzicj.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gwhhthvug.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gpqsmvomg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gexdhjqwq.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gmlascyrr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gryvurrip.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gelfpbwuk.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gtnvcbsla.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghhpjjyyx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guhmwxhls.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gvktvzxgn.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gywvmwuxd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gvfsnreif.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/glmskwntl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gyhlvlfbg.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gglalenjb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gtfrnyghk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gozvztarm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdweitqqp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gbpfstsmg.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyonxjuwe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/glheusaba.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/ghhqrlqnf.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gextrzwxq.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gosolndvb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gbtfsmlal.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtosbrrxt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnngrplhk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gsyndazia.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gqgzquwnb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtprmhdvf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/grhvtbqaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gzqadzdwj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gkvrlppbk.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gnynvvrsa.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/goweovlzu.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gkyxjdxkn.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/geekuuyjg.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/givyjflgy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gyocnertc.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gsptsrshe.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/guiwtpbll.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gvbywifkr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gooxgbhst.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gswrgcwca.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/giztufgna.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gumipbbaw.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gycbfnxcr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gelprhifk.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gttvwwrsl.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gvivummxc.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gmlcpjewy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gnkxrrstx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/grrmqpybe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/ghwltcvgd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gjickouaz.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/glyweqhif.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gateyrdde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gwpsgbpha.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gbmalfqvu.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gwlbyvkwk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gqlyblnlh.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gmujqukly.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gvbahhcxu.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/goszxvhcz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gfcwdonhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gbarnuach.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/ghqodpbdg.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gqwhxaxsv.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gkkhkmjlv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gppvuhhda.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gfspievrh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gfgndhgqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/guscedpmf.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvdrhrrxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gjraeshio.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gdoeeyzhb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gdzmrvjie.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjuxwxfwj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glvkoiguk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggctggkku.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/guxiaihxh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggzbptclc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/givlilyvv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gilqqzcul.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gsduviayh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gofomilnr.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gmyjtcvmi.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gfcxpjwdt.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/girmsrtvr.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnawabpyk.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqudovncy.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjvbjusif.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gufjwsjus.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxseqmja.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gegcygaun.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gacgbzoto.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/glvtqcmph.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gmfgffcls.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gsuiutfqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gtljpgdsv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gqvjqxxkq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gblnmjarm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gupnvwbiv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gkaufedwy.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gzexdtvte.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gwzjgzxrl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gvvkysdws.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/givfhnfwv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gtefdwajr.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/geyuzstit.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gyuatbswq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/ggtofbedj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gthiwgryn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gfqykqrju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gggveqgnl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/goakoaczh.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvdckjfpn.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gutsgragw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/glnivbnil.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gngrxrpex.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/grxdsrcqf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/giwizeyix.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geotbluxj.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gcwewqaen.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcokrmkyj.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gczqpbunk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gpjdevqfl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gskrkvtom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/guggxawno.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmmmsvlgh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gzbdrpxof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gxycewzdl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gommdnuld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gaseuyndj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcfwkmh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gggttctey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gpnthjrzd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glgncigpg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghdwsniqn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggmprmfnk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gemcvdzob.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gcmicsjpi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grtbbcdid.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/goeuqegwg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gneougpmq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gvvvpzrbe.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gbgegdycg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gipwdpgwb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gewdhlobh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gmhkwsuxc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/goeoyuiki.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/guwyuxlep.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gzxjfubky.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gkpvvitbc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gtzqphiin.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gmgszotet.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpzngxswp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gfhfhxezy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gywmrnkli.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gskxwdkiq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gysglbeja.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gytvzlpcv.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gscykuvxr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gjvixpnkf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gprrtbnrh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/goxjlcbid.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gesgpeyaw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gbhfzrwho.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gbimjtldk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gkkvtcyfd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gwiomopwq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gbcaszydo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjykpsim.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/govpkhmdh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gaqshgbju.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gleqxjblb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/ghucsqkii.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gxnuejplu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gvccwvubm.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gsrlpyuks.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gukfmthtg.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gohdnhjsy.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gkcekqgad.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gejiemvgl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gxmcmwihg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gyfaogyqs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/ggyxmdtfa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnyiamiqv.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/guzypmsba.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gjsruivjf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gtbqfqkvo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gtuoucvtw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gkptnhqyr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/grskbladl.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gihyqtohb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gahyfnnaj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/grwgmfgjp.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gytwrkjqp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gcgvrxdug.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gsdnunmef.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyibthsw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gkuqvahgn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gxexabzzr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/glpocxvdr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/ghvxgqhbw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gopsngsgk.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/glqkapqyo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gjtwhxcwu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gffwfzjnw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grdldjrwi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gvmjibdiq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gtpxkeuti.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gnuhlaaim.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gcxrsslcs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnnwlzwwt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnuhzayul.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gftpigmsq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grhyuvwnr.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/glvgjktvp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gaknzszgq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gogfnaban.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gxbtmvrxr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/grjvsouhp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gbncsflkt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gtzjlcigv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gamvnzxif.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gowqvuksr.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gmimahtbz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gqxlvcwsb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gsyoacihg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gcxqthjfg.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gxxoouovr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gexzyfept.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gyovhwjus.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhnzcwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/grlnqczdm.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gxntdrvqo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gaimlcege.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gpktqsfaj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gaudbgfin.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gcxwqfclm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gwitkkeiw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gkhjvbnlb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gkibsyers.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gjfsfzunj.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gnnvirfew.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gyjalugqi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/grkxkeyoj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gjainhiht.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gwvliywyz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/glwiundou.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjzqsapny.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gflnjngau.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gevawagaw.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gcwkykqfu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gzxydgmmr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnodduxgy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gmfsqipyo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gxpjlxpij.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gvhrbwepf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gmdlogdil.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gbfyxrhnp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gtwtfqdvh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gimmmqwcw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ghhkbxtxt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gyawfhynk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gwiffxptd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/ggaazdfpf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/glcigpukf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/ghuzmuylk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gbbhfdujr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grslexive.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/goadrcjsi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gztsanpzi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gzbsbbaru.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gshnukede.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gurewudvl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gkoeecnzj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gpzosocbc.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gmjcjbppy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/galflerwz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmrymjb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gdzzfegrp.sHtML


<!-- 参考信息 -->