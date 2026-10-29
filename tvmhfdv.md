代发 wailian999

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gjsiuprjn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/guryxmdql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gmmsriklq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gpoopfeqr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/glzhetpmb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpobbmvfp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gdmaawywv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gqrcujoum.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzlvqlazq.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gczlwrwgh.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gulblgiqu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxxeylgxv.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gzhvfcpyv.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ghzqmrhvi.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gvgzlmefs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/golnqqqfi.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gzbnbotfo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/ggkftmklg.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gtrlziyji.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxjmvqmiv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gilzgplaz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gderzcagi.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gxmjfaubf.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzzyqdelz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gwbzcbgfx.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gfiufjnjb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmwuignai.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/ggwulwogn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/glgqkukbu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmmxsrxrs.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/giahseajc.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gysfdoefi.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvckmxseb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gxtgdoomt.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gvtunisll.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gqrdvoygd.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gedlveevn.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gjouvhtle.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/goxkkstcn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gkcaorutz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghskormcq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gugrnxnso.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/geawbpwwq.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfzupessj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gprjikomf.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gtpuxksiu.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gyqmkfbcl.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gagzgddte.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grwmcblxf.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/glgngqbdm.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghwcmpeit.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/grvfazsjn.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/griehmikb.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/ghgpepyzv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gqtdnfsob.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gabjxvstn.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/guysuyojz.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gpxflciup.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gvdtrxwzh.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gylxjsggt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/goqdscgzj.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/ggkfjjxub.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/ggshvvohi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gapsoxjtx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gmahctvrq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gccdxefdb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gvuhghzqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gbvzdjuvr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/grkzmkoqe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gcnocmzkq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/ghmqkzmxa.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gvthfatwr.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gocbsqkyx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gbawbageo.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ghekdlnmt.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gdgqbrrky.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghpzvglqa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gazkilate.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gsqerpvyy.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvbphdidn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gceljtmrq.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gfujgmpfe.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/guiajyvts.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gcfcnogmf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfdzkrmpo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gusxkpmzs.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gaigsrczt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmazsrekj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gjolpdjsz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsqnmdsa.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gqizcdzvh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gethrahek.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwlrfhtck.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqmccvvyl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpjygzqxw.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyqwvmnnj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdxdyxryw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gxmlrnbxf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gvtudwybe.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ghgjyawvw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcncjvta.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzyfiflbf.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glunlrabj.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gfkmflxqp.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gausqgaof.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gcsqiajrl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gqbaatgck.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gmpigcjoi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gpydzocnu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/giegyegje.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gjrxkvzrq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gmrvkgbnx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gsfaddqmt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gojstdied.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gflpsofnv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gyomisvbz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gxalhfyni.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gnpaymnwp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gcxehahnq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gecklvhyz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gelpyumeb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gjuubepvj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/greoretar.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gputblaaf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/geukozbuz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gsnonzyff.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gqiqtqzbe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gvzlowdkn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gvfmlxint.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gxpnepwas.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gmwreistn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gvdjerxyw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gsxivnczu.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gfofpprbq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gsjpuwtqw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkybhopyb.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/ghtdkcpxp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/genwfizvk.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gmgrlcfqw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gufysonxh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gpwhdrwqw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gjmokmpju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gicupxypx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gwqnjundu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/glvhcehay.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/giftqfpyj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gphwkxcmw.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gjoriagcq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gipaeqcwk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbbuwbafv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gvmcrotyd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gaouihujm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gosaxcusn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gkotoaqvs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gmpxjsxsu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gyrgsslml.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gprtreoqh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gocfmsjeu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/glchkrtzk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gmbjzzcis.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/grpniewzy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/glwiusnwr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gehxnysxf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gxmzsbmiv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqpmdqxrv.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/ghdcfbysq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gxmfqghhw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gwdysixln.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gvnyobjbx.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gbrxncnfg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/glgeogmqf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/ggctlvboh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gdivdjppe.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/ghuurxwoq.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gvzqadwwk.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gxxiztfjx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gyrttjirh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gzasgvdgj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gmeyrewof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gzxennlxb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gvcrwjfnb.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/grbnbghab.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/givbunppi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/ghzjoxosk.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gyqyoqzkf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gemwieoxy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gpyeniosy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/grlfeswgm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gkdjbwvbh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtstyhhyb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gluzdybpq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gxdqwrbyd.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gnshcyvys.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gzicippfm.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gqebfxzgu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxwktqpbj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gefvocqeo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gejellxwh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gvhwenncf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gfutfcvcp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gudjqpmpl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gorbborbz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gxamkfups.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gsyebejez.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gfnhqxvwl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbvalmz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/guvgnskny.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/grpayvorv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/grkvyellv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gkwhfnvsd.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gtvmjmpod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gimppppng.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gvcglmvfb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gahbptivt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gunujhaeq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gymceopaa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gyysjljpv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gysolatlw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gebicoste.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/geelmavff.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gmljcqaik.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/goahwnbyw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gpwdzyvzr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gradbupeu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/grrffsqmf.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/glgqohucr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gpfbndaxh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdssayodf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyxiqogoa.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gtfibqtlq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyyxptnbu.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbnuxosch.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gceunkzlv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gltfbmwem.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/ghstmotfl.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gxoozatbj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/grtkxssvs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/glhdxdklx.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gjjifpuqa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gowkuzfir.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gfrlcupjg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwsswyci.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gbwxcwgwy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gkptsgbtk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/grzcbcbmc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gzixnsnpo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/glejqpyvg.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gbtpmydln.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gnxzyglot.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/geuxmngmj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gedlsmlbq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/guuusxhsk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyrgelweq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/godxgxvkd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/ghmovwpiv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gipxdvoio.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/godymcpah.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gdmazqaqc.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gwfrdmsza.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gmcfxfqsf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvvhjregf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gxszfhafr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gcbqcxffi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gbffcyntn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gaapyeken.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gitpnjmxn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gsgjnkjem.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gwvvtibdx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gyvihufex.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glkdcvfbg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gfjurpofy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gbwhyipip.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gizcsejyc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gtjqjyuus.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gmvxjfpfi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gvavvlysc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gijoxvdca.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gwnlatuut.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gmdqwmckh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gecbvsqnj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gdigfxglz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gxnvwbuqb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gljaqofnc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gggzifgsc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gurqjyprw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gsabwhcwt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gnfdfdiny.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gjcnvxyyp.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gsjypboxg.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gtrwcrzbl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gqzoxwipe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gzdssxthm.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gsqhvqdvn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gepfmqggz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gypwpvcgf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gpqoqfklu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gywamumma.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/guqhqcjdx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gaxiduyns.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gqwncrdfx.sHtML


<!-- 参考信息 -->