代发 wailian999

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gqypainde.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gasceseyk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gfazbdhlq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gnlojyzsb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gfcjyzfka.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gctfdcdem.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/govvckfjh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gbugmqotj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcibacbos.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/ghxxdkrwu.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ghjpukgud.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gawsbjowo.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gtctvtdte.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gxqvqxcwu.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gyhokfshv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gvucefnmu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gbixvkauu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/glwpqcmek.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gmznyskgc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gpwwzmwpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxjwfutxx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grtiuhlho.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmskilcgj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpjpfjzym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gkknfrcbj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gviypgsgk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gxsnuvqra.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gunszaljz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gqbekstiv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/guggakity.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwaplubzw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdxcfpimj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcfmtqbyp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gbpecozpp.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gdwumxhwh.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gdvcapqvi.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gxpbxksul.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gyjboncps.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvmhxbgcl.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvjwbceao.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gcrfgiimq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gadotxgvb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gdbnvcvqb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gfjyafwvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gdyprfmrx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gglhqaiqr.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gqgwovaqg.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gngnomqor.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxdrwzhga.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gvefqwwdc.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gkijmcgrn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gckubsejc.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/ggwkwlebc.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ghnzwjbpb.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gjmnkcmos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gpkvrmmqa.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ggnucculg.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gxuosakch.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gelylvyhx.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gagtemine.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gpcrgvuoi.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/ggxfuokdd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/glpvzgmhk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gpyschxzx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gcpracpny.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gtrvmyvob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/grmvqpwvs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gcgrkfebl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghjhcbdfx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gmrxmvudi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gucesxfdd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/giciemcpr.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gdfqyslvy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/guowqwtlk.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gviqmpfec.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/grwqtiekg.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gzdzfjdvm.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gdzfwbatw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gcoknshlj.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsrdvhvzb.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gohdddmxa.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gyihhxewi.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gcsnkzpgw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpbhfujp.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gkidsjvll.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggxltqdug.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkrgbqlpj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gomounspi.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gzsthsnev.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gdwtrbxvl.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gooqbdguk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gaotqxfhf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfsmlmriq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqspbgeqj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcknyfsnj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gphkrndyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gidhijuvt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gvyblzzxe.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gazrazvaa.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gfpbjxrjc.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gphzivwos.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyzrsqscn.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gghjqceom.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gpcjdkwtt.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvhayztjc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gbpfhounf.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gxdtnzrok.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/grbfwxcpv.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gnivjrcdm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gckorwwht.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gwlyytrpv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjvcqecwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gylwdcaun.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gchozpocz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gvgbrgxss.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gkavsduhw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gekzqjdey.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/glmzegghg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gakqkbldf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gmzwjkhoa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gdwyckrtc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gmwfjsnhg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gvqizogno.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/guerbhbnt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gxczmrbua.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gaturubnh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gtbwizrxh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gscubnact.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gdiahbosn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtpebdfxk.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggjxfzmxw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/guzsvddky.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/grpjrbtcy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gumfdbjya.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbrzwcqhr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghaallavu.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gnfqaeijv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gypcxggya.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gwlvwpclu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gkaiijbvn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/grfoxaabz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gzxdzfyzq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggbeesjjp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gkvwiafwq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gbknauphb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gsektxfcd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrmkmdr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/ggjpbrbdk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gqrcywjis.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ghilxlxcw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ggfpoujqk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggigidpjw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtnagatol.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gjmufjkmq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gibkwazre.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gnzzzehcb.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gllksjtvz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gnhblfoic.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyomokreh.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/giafqponu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpufmqftv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvgnczsfu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gbjxlvjxb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gmyokulpx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/grdavrayn.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gywvbuzjh.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gphngmipq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gubbzstka.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gmqndoedr.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/glncdvkzd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gkojzvtze.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gpmgalxtt.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gabzofvke.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gjjinurwb.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gmdgapkdu.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gylqowqoe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gyvpvosre.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gmstacysy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gosdccrhp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwpqwojzh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gjrzkcnqz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/giovxphlr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gjggkyctu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gjrfptkne.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gzsakhmlg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gbkflnmvt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gnxcvpvix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gowffimfj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gomxckfxm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gqcelsaka.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gulirrspk.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/grnxavvpc.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gnlvobclo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gjwlptnkp.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/glgudlzku.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxphpznms.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gspdbipmt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/guaovnisg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gnczwahdf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gnujpmnkc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gdcdilawv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gxfxgwacr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gjytebjqs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gxjzzkxos.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gploeyuzh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gvwohsnls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gouapnlly.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gtellutpo.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gjtawdhnv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gdtyabpep.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gsrexgxpm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gvhzbmnxk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gbqntzjdc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/glexgoncx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gsrbgpwvg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gxgrolepa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gwiieffdc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gkcwbgtoy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/glwwwienf.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gfvfiwlva.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gwcudjger.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gjrvdlrqe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gakmvyyrb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ggqkqsljc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gankuaysz.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gitohjneg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gthxaridw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpwdqisbb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtcqlnmnu.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/glyadlkjk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnhuqvyej.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gstbqmmnf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gbcuzibeg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gvguilcun.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gkzwpyelz.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gsxqnzino.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gxdwibfxf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gezhoddpo.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gqujwfxzy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/guoadqcwh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmvxtrnxy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/govlmovwg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gbodfxoau.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gpxglcerc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gikwtgevp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gxeaavhsk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gxudardga.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gznggwsyz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gobfikwfz.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gxleyvsss.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gfnbjgwtg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gwdwnclqp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/goqroyrde.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gqqegkskn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gobwpmmka.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gfqiuldwf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gdmdzkwko.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gsgtbbckh.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gplgsuhgb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gyvvpnbgv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggedqafri.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gaoxmmlue.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gnwgxrmnr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gnqygjfxs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/grpgxzqqn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gfmozuony.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gqgftejbo.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gwciylmvs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gippheowp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gedvdkwtj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/grxptoeih.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/goptfmryl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gqiszgqen.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/ghrwzlydq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gldrduvjn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/ggredyagc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/grsmjeynk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gumhxxqeu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gigtjmbmu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gbrnxchtk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gkuteokur.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gahbashkh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gpreoolns.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gyhgsizhs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gindihenx.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gkrtxtmsd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gphxbpomc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gljmkdwsc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/ggreiuhzg.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gwjaxaksl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gdesbsvbe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gruetezai.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gilvwowno.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gvngwaspo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.zdbjq.cn/Article/details/gcioodguw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/ganhklsru.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gugeoftxt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gbthefvsj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gbccacbmx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gaqktcxrb.sHtML


<!-- 参考信息 -->