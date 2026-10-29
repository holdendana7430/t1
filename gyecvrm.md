代发 wailian999

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gozvjhjmy.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/giuoivxcu.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gmwqajxpx.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gohxvpwgr.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmijxgrsc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gygnvkqfr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gjikcgfvi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gjlabvxdw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnrhjnjmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvsisccge.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/ghxxkqyah.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gcshjjrid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqzxjqrny.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gvsdbmlxv.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gwnvzfkxm.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gunphdmfe.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gzddyfacb.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gtgyfrulm.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gzwnnkkpw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gvpbipegv.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/geinfkmiy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gxdyjfaon.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/grvsqvzoz.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gihffpbgb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ggjrxbwbg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glweveefe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gohkyadao.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gayvkzvbp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gropaqkct.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gtumytngw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gpajtwizi.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/guqjbngml.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/geszxekbk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyykyunkt.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grszfpkpv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grlfddmtb.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggpxugbab.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gqukjvssl.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/glynbevqx.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/glqmsbvgm.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gesspqthk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gybitliuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/giylvhbpq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsaylpiyt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzhsmrjpu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gpjmacrfi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/guuqmodgq.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gvypffetx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gfgxlcugs.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gmqyzleyw.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gaiuxlhaw.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gocaifwzy.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gzspmladm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gcuysuanc.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gsraiciiz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gtcjmxqve.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gstaluokc.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/giqgwgnyu.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gfsmhhfvw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/glrqoihpw.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gqvgqrpky.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gapikxpwx.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gkuhbkenh.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gmysuxnid.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gzctgxwas.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gdajziapp.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gvzxphrjf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/guelxbiac.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gvozpzitr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gqqifvaww.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gqlffnekf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gujefieqf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gdbipiriw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ghbwobgpv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gztzgkzqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gonrpdjsn.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/giqqrzrhs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gkjdismza.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzcdgotwq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gduirzeyc.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/geqphtswz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/glzzlvflq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gkzgajcqo.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gacjjpixu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gkqylvjfb.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gvoacahbw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/grgytmynm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gnfyitdlh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwaxbyi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/ghyrkuova.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghziifuug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdswwcttv.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gopyocwpy.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gphkdtypp.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gudgirpue.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gwfrafbwh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxipfyh.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsucafcxl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/giprupvku.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/guklokrfv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gmulphrtu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gkakmjocm.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gvlnnldcy.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gzvbicsgo.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gsdflciza.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcirorkod.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gitamzeqr.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gutvfiyrn.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gqljspgja.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gxetozjfe.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gyriczddo.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gscyonosr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gmfitocuq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gzhxkboid.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gkdybpwtu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gagiewiuu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/geauhdpmy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gwtpytfxk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gzunvpbcu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/ggwhutrnt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/grtwwkwmp.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/ghkrouhct.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gkhuvaqyj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gwepggegy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/ggmepiwwp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gihcctkjy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gvnmnwmsi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gcgfawwft.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/ghlgltjht.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gniwetpqg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gsfflsoij.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/guljaqios.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gperdloco.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpsbhdkpm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/goglweprw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gdafztrbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gprrodfvr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/ggwcttftk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gbpecvotx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gntieswna.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gwsaiwmpp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnphluzyj.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gtgwblcox.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gmgiwirlm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gkcvlkbqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmfspgozs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/glibftkic.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxrbubshw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gvfqdykzr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gndgzqfhl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gpzmpmfkv.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gstkefhjh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/ghzhtvagj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggdkylsmi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gozltsghi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goplkaoof.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwtnxcsed.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gpgegkwjb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gplflngaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grkbhkirs.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gbcfxfrth.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gwzhfzlsw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzxjqyioq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfumlcpte.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjwmxcxae.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ghpyidkmh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gmbmsdsde.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gaiobuxvt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glbntkbia.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gwbqvhbsl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gizbxzjss.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/grmunrfww.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gqqxolizu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gcqwgmxqp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/geeewkgee.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gdysiuzxk.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gpsgyekdc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/grmzayvvw.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/grzuphrev.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gtxsmlzva.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gkdeztzyg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/giekhvvjv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gmuivswzp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gfhkuycyx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/grnjhgcul.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gmpfsxltz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gkjpahova.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gixudqyrx.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gjzldjcdp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gvajtmgjc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxypuiget.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmfjhduff.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gfhrdhbmc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gnxddzjpu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gppnksicn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/giglezgzw.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gwmsxihfo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/ginilmfts.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gzbausuiy.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/goxqmigja.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmqgpgsao.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gdmthbiha.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gsmungkwk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gpijingni.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/guwqlwqih.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gayaopgxf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gfssupinf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gyjgbdgid.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gtjxhykst.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/glugarfdc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gzsznadcm.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gbdnscxht.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gzizyyblt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gownmyssr.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gaubhgjix.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/giyoiodjf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/ghpqmzxbz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/godjrefja.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gvqbjsldl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gjkpxvfwy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gnkxmurnw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gflepgalz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gwmpvfift.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gubuszyej.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gujhkljoj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gtnzcjhqy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gesylprou.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gaebzbuxs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gqhtilmdj.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gnneevtzk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gbirwmsla.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsxqigqvu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmdejyjfx.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gosbctdow.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnknnohsw.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gynqdnlbt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gqeoraluh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gacyxglzy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gheyovcgh.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gnlidzpzl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/guhnsynfk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/guopvhdvk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnghxzlly.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gvicnkidz.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gyaludmkw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gminhuxzv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gxlguuwzg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gjohimqrw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/guxkwpaic.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gcghmwium.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/ggcgprehu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gsxspyfou.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxrusouvb.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gjyncqmgh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giavuxzwb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/ggxjojaeh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqtdouipk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gnlofllfp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gwwggbqwg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/gmklgwctj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gldvcdtqr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/glpbtfuvp.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gugiycpid.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/galzadukz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtmoyziyl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/glsfbwtmr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gfnboxnck.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gsrcvlpgu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gfrulqxbk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gkemtglot.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/grhajdpig.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gsubkvswa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gqhyglqac.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtmfbdgdq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gjvsyrned.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gqpqetusp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gtlmafnll.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gayqqukgt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gxsemprho.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/ghbqinuza.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gfvxiwchd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/grrukdnrh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gwdqdyrlx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gpybmbbxc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gdzpgqewp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/glohcdhft.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gmlnzlkba.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gpwvmptlk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gjbnazlmq.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gpnalzvhh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/grilexawy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gwuvoelqh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/giqbtiyyv.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/ggwijfqzk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gltjtuivj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gehwrqyns.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gqbshuglk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gzxrkpuxo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gapgbekuk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/gcjlmaljf.sHtML


<!-- 参考信息 -->