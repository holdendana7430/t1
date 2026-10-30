代发 wailian999

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/glqzlcgnf.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gvuqzuwwv.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/goaomluhq.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gqzljsnxg.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gboajsbis.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gyaxcmojg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gkhwuyucp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqssoyqxj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcdgldhqx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gikskxcoo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gcymcgkpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gmduvxzsh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gutlegjvd.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gvjawzsjy.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gjomwibvq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/glvdllrxu.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/ggikciqak.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gyscsxfym.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gtyqizzkv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gkwfeifyp.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/guoaaoeps.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gzdvooskv.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gydtqzpkc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gsytwroot.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gapzphpyn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkxnsrkqd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gipjcigua.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmkkismym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gvhfulojc.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gegqyzdvk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gnmteyucv.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gqfhqjnld.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gzimcjipu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbmvoxcdr.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grqfwjzlg.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvlhdbjeh.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gcsczfusf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/goguvosfo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gezazdffh.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gljmnfpac.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcojdzp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gkzfowpzp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfrivrwsi.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gcpmqglyw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjqjaks.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdastlouf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/goamjkmjh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gzmqbamfn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/giezjisbg.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gxsslozgr.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gcohrjvqj.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gewuhyiiu.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gxlyvspwm.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gxzctysrl.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtnhiucjm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gboulivni.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gkxxnpknf.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpumhyorm.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gfxntorfj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gzbxhhjlx.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gdspmoayv.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gullynuyq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gjebwgwoo.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/ghkjlsmug.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gigufmznn.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gaqxeuzom.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gswvxhrqh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gqrndkycj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gihefloaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gutqcqxvn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gsztaognp.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gbjepfwok.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtystbqkk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gmabemvzc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gpgdcctlh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfrwertnx.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/ggmwrqfkg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gbhuiwero.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ghqiatjue.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gurtykqmm.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gthxzkxpy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gdrfloofy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gbipradbj.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghnzbxeec.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gpppbczvl.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gyveisegb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/ggwqttgfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghmcwgkbx.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gbrhfefyw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gbutfeuyc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjpzkpkds.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/guaorriac.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gtzpwgxrb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdynciigl.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gtqqcwqtw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gvchdayzl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gghfloydj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gccqbfijq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfnrvzdom.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnwtfmoox.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gauelgsnp.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gkjqhemvp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gddptjezt.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gwgbfdoyt.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gtwyrvwpz.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxfowjwbq.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gufdylinl.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzpkaebtx.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/goovdtmar.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gukksscmz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gvxuhvjut.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gysfuaviy.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gvckpybai.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gaxhpdgxg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gwhhmvfti.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gceuofezc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/giyfcdmai.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gxluulxjy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/glegajjta.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gdrrzfuqu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gqqacvuos.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gjrsehqtp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gacxudpvl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/grdwlhghw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gmlolmabn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gxqkwmuzm.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gyghluity.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gususkbld.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gffnvspsg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gwxerpuqq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gurdgeodn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gtngqlnyn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/ghyizzhzl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gxvgfjcbf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gisvblrfw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gkhswhlzg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gqymwbchg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gcmrccgms.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gagxrdxkj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmencznyr.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gsmbcagou.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpqlmcnws.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gxvzprynp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gmaxsmmyd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkyohujlk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyuofmubc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gcvmcwryz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gucwkbmoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gumgtstme.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gtnefqmth.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gzpwsotzq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gkvezgzwr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/grgliavjs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvmkbundc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdfhkvfpy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkaponsnk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdmzfajud.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gbvjijtdm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gshuaxgrk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtfbicjai.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkmwsulbr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gxvtscgiw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gshdeqbgz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwqyhfurj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gintfhhgd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gjeqmyzke.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gcblduikn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gqzqrtcbf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gpmytkdtn.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gkzokifbd.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/ghbasrrxa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gmgrhpijm.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpjlkhznx.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbplnuoox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxhzqyymh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gujmkbxmd.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gzawkndvc.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/galogzihw.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gxcwazval.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gpgkvtdhg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gdfzttzpz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gurjjswgj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gntqmbejf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/geauztmph.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gkyclxflr.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gvxubyqbx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/grzoqnxvd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gkitgisdw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/ggvmyfork.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gexiraqpu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gqncsuldq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gdoopbdfd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gsksnzecp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gmymfique.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqmaxmo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gfdoafbkm.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/glmerwcyp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/ggiflroiw.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/glxgvmbqq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gykagzupj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gydzmmxkj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gwdfphocf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gqbpcfqhx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gqprdwwfe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxrhpqkih.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/grqyvvekn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnyfznf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gyxevcwnw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gmhhmkggq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gxwqljocn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gpshcpmhx.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gmdgusjnw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gflwpghkk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/giynymfbp.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gduamoroz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gfidokigr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/ggesgfcro.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gdlbyjrjb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/ggjbsaqpd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gbsvwrvjh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gyrfynrkn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gkfznqibp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gfwetelce.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gdzeiwgww.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gjsxfpnfu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gxqpqbcsk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/ggmgycqwf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gmmgvqzmd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gkkngaubh.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gisbqmixz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/getsxrhyu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggvcoavlb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/galvqszjk.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gctawhavt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gguwxbqkr.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/ggyrvwoek.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gwkxmrhxz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gulloumcr.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gvtjdedlb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggfziwjbh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/glptqvciu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gejzdqplc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/grgmengat.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gtogkcjhu.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/grluzkuhr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gtxetpdph.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gfhjnrflp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gvirbgwmj.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gaiwadkas.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/glltduyaq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gfzklfpzd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gotffendw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/glhgdkmeb.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/ghjspfpcz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gfvexuupt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/ghvjglxvw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/ghcyzdpcw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gnkibxauk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gnglcqdrk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gzpmnrhod.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gtrifukli.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gssoqppbn.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/golzrniwa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggjtabyjb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gblgwqaiy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gysmxqdkt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gumwmtpoi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/glshcffmp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gxmvcucoo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/glbaikmai.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gbpfujntd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gcycvtbji.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gjjgvahgi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gadjmetwi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gulzcoyji.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gcjraxhpg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ghrmmrhqr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/geebxrcbm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gisyordfg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/glevaezdf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gbffqsotr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gdawmekrb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gqqqsgdcp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gsblqjmyu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gofnpcnkl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gcroycggf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gjqupozvq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gxkvbwaan.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gipnqnqlh.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/ggomxquwt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gdvjmnifr.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gktatrjxy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gckmnzlby.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gmprcgkpt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gjibnyvgo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/grrdzgegx.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gneoizlhd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gkckwdqmt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gizlmowst.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/genwwlnfd.sHtML


<!-- 参考信息 -->