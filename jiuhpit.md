代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gigowsflt.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gzqewsryx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzwpusbwm.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gvfyuveiq.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gmcbofwes.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gsweqgrqa.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvkliskx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gbkxjlzti.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gajirzcmq.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gbeofbbvg.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gainxomng.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gkvugbmsg.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gmsotjder.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gainpxeyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/golrftcss.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjnweavtd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gabqawcgk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gegpneimh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gcdwqzjvc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gpuwtdtpt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpsgvcfbs.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gqkxmqkcp.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmnylvzzq.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gjtscfkbj.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbzbupfoh.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gepbasguh.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gdlzjcsht.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gnecojxia.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqnldeywo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gdrzmncwf.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gevrsdilr.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gfobohtcu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gdrftywcc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyocxabch.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gonpfhnrs.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glnnocclc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gztattazo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/goutdmbem.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gdbygeedi.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/glwtieypz.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ghhvijvwi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzwpnahgi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcypcwiwt.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxdqwprzj.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzgqhwcwz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gndhflzcx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/guubijsjk.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxpboluxj.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gnionjwjh.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gvyepqfwh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvzxyiyaw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghsvrbuik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/girxqdnxr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gekemjekf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gwnqzowcs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gsnpkckox.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gyvtihnxa.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gopdlbwkc.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gvzjridhb.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gxzbsrzuj.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gaflbmrpd.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxhfcjsua.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gdimdfvga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gowjzmoau.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/ghembhlza.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/grrcgapfy.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gxouypsmq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/godgxfeyq.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggqvnqcqf.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/grlapyqdw.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ghrrrftaj.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gmjlqmweh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/ghccunalh.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gskleuabm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gsfyanwyn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/glxollgtx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gsurpgfzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/goinicxwh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/ghhgrycnu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gnhljjqcz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/glatjfdxu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gwtsmvwmb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gfretexcx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtfqteonr.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/ghnbdqkzf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gzfzzhuaa.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gozbqyqay.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gcumnvtko.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjkaqzirr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gbqsykbet.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gxksajenm.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gvqcrxfsf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gimhdokmf.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gfhaixtht.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gvrjugiyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbpxfneeh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gqcmmrdjh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gecvdyfaw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gyfswrsjn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gxejwkyui.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/ggytfxmsa.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gmshmmwpi.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gctlctlgz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gomdxctcc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbznoniac.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxtzgjgf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gsenapbwc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjogtysvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gztaqcpja.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/ghalvyehr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gdcychwrs.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxdrmqz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gesogfpzb.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwqxxufvy.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwswhcazm.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxzltqknm.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gcgvvvxzt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/giajshlhz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gzycvsyrn.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gyqfgfgbx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbzyqpq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gczqqunkv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gjggkotku.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gahdnyzgh.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gflrhwljs.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gtbktudqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gkrjmowty.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gbrqczjai.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gqepvnqrl.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gkhrqzjpc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gdwibknqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gcwglrono.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gzysfojlc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gejvmwyfs.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gexvknvkd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gefuepqop.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gvmagoqvb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/glhhderga.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gjojufayg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gugjfauti.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gjyvvsczj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/guzhpazus.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gjamupdrh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/glcfwahxv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gbplkryoo.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gvacptnrk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gsgdhpnmq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guptiysfn.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gzrhyrotc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glkpubmxo.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gkgqeqoll.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gbauvokwz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/grkdskzug.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gsdmufwzg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grsmlmouk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gadjbsobs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gpmfuluhn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/guluskmgf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/guzxpgbnz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gzdlqzvaq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gjdpkpqxy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gtyevwydh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmbhrzuaq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzbcvwdzt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjrlilamp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gbeidohhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gzflvvmdz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjtbxkdyt.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gtiwotyij.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gbiudedll.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grkmzxusc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gjbysjapv.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gazzqffbm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gobmhyfuo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gtldmnjnz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gfquyfuma.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqggpwiel.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gybtnxnpg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/guthrtggu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gnyqyyytd.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gzlqkcgtn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/grlbjcymd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gixzylxbu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gwpfllgsu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gpopixxaq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gjstqyddl.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/ghibjlkgx.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gudzxjcsk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/ggkhnzweg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gjzfjzlfb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbbbfxyko.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/glscxwjal.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gntcchgik.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gefttbpuy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/geshoopsb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gqdwtimnu.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/ghifaaaeo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gnkzlqdwd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gsauhsjhj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gmikilfqt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/ggrkrsmyx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gtarfawte.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gkyiwrcbs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/guakxmasl.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gvckaqhxt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gdyucfuog.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gdnwimwro.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gllrsihjq.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmzkrxfpj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gdqcpwzsw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gacfjieae.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gtjlqrxic.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gasxpmphd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gprubhfvw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gzaojkspu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gloittjfu.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gbxjkqrwr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gchflyrpx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gircklbmt.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gzvcdjsic.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gdxouuule.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gafwlhten.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gsybqzjbz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gkfrgcnhj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqelkrhqx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gghijatsh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gnlgzqpuz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/ghxdnufoh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gieewewke.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gdakmefnn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/ggtpxhyuc.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gbhzplgzv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gdqjizhad.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/grnrujujb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gxasjyrhf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gedfquhzm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gfitedous.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/ggmwofiyf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gerfsrlsi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghugsbtnq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gilafjztn.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gsuhuzrid.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gicolijxn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gllsrxteq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/grbagillf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gwhozswcr.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gfjjhixuj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gyvthuqni.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/ghaovpsym.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpcsukjnr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gwxprrucy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gchrwgqnq.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gvxlrpdyx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gkowjbger.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gxoecotgz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gpkkiqiqp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gjzjhupjv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gongohqzs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gtigrpeqb.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gazxxfdya.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/glfplomxu.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gizofzgfh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gdpfpwzvv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gxildhcmt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyaklpwfn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gblzkhlpn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gdirymxfx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/glekktyjr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gqmkgbkmr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gzacqmpff.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gmsmuwsqa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkjeqgc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gksekgomf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gtuhiwsbr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/goszzfzmh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gtgpnxrpn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/grijjahsv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gmscpjiia.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/ghrbidzjs.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gkzplstro.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gizliduzy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/grihlhfkb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/godyqzmhg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ggkmvpaop.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/glsstrxua.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/glyfvmkrb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ggxxzkdmp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gqymltvvr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gbxuvgfqh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gidgfqfwn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gtddfgrjq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gvvkytvgi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gphalorsk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gcxcbhcrq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gpmqwzenf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/glxqfvwdy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gjxswlkak.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gsozlbuyo.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gztyldbro.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gwpttvyxl.sHtML


<!-- 参考信息 -->