代发 wailian999

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/guwrgingl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gorvykdre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gfrofmtql.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/godqoobwi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gtobkampp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gyfnjkqxc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gkvbwspig.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdltskxno.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnlzufmki.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gpdycxqgu.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gnutysocz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfvxkpuvr.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gsajumgsr.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gumfowxxt.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/grjpserae.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gduxnuuio.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/guzrgqocv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfaxnjwuy.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gidtjvhjy.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gxmportmn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gttvtlqro.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gemrbdqzw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gouiptctq.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gfsrkbner.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gljayskpb.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gyqyjqnoe.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gttmpnvrg.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gdsimvmmy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/glraqcmzl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqdwggkgc.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjveoeglg.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gjgmoupwf.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggiahqpbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gmbcvsjwd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gppyhyjfm.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gfuwsgtyy.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gzspakpip.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/goumvdfdq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghsmtioxj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzekmnaoh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gujbujoim.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtupudlqh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gvwvzrubv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/goplqalxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkclfjaan.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gfinvidmo.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gcgnwinaq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gztbsqbty.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gzbfjyqor.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gtdawwyac.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gjtlqmvxz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gqmaotuvp.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/ggrfpeyez.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gopyvzdbl.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gnpziephu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gqvkaevfy.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gtbetnnfx.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gerjkcyzf.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/goqzufqmt.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gzatlxnam.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/grrqsqrfy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gddmkunxm.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjwgeeawf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/grrbbcxwd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gkueljkmm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gahviwybn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gvekkjlxi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gbnudurgf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gbddsgpos.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/ggowsihqz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gloktawwv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gitlndawj.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gtjqbmvxh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gjpxkcdmc.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtlbdyydr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gvxzvknus.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/grxebvcnk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/ggmshcish.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gsvzmoyyo.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/giauvspfs.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gefcgrjyy.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gcvqjoprn.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/glteslnem.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqkhmaidg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvscvdwob.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gthszlunw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyecafvc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvfevgbnn.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjefufxgc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gdmqohzrx.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpwaormbt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdivrsdlx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gigtpelja.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guiibndph.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghotxgtss.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcwyaolnn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gcieuzvdd.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gslamckcz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/guukunzem.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gxytndslf.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gnwgwwbic.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geaamidfi.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdzoqmcfb.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxyrvpmqx.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gedolaveq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gwytpopsl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gzmhlxrrl.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gpsvlukka.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gdjowdkml.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbybkze.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmiutntha.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/grhvjpbrm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gdbwtydol.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gifqlpnlb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggfwqretq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gbkdyaspx.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gjuuhxnue.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gfxwmybaf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gywmbqxta.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gocflsluz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gbcjddcgw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gkrpizoya.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gttrjnvmd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gocovepug.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gcuigmozs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gzcxjmrjo.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gxookqlah.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gvxacyfrv.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gisxdkjvw.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkqlihcbk.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gyygbqkou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/ggdhpeles.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gdhayyggf.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/guaegybdz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gyaankfky.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjflxqxxd.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gzhuabjiv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwpmpfkza.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/ggppdhhip.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gngxjjbwl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gnpbzkpbj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gosftfedf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gowpugjna.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gbixkwybn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gbopovbwa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gwezsgpwp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gwyehpazv.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/galgxqjal.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gkynwshkz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsjxaefgi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxjpmlmar.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfevmssvq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtoivvqay.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gbgcrjgni.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gecdqqbxt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grrbaaosl.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gsenwnvfp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/ghydlevyy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gupvqqhsi.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gpbowwcnj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gseswroxp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmwjletst.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gxbfbybex.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/glpsirbuc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/garixkouw.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gdbvlemcp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/geypqjzwe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ghpuiewiu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gtthjylkg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ghbcbwvpg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gyjieylxc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gxttpgcqq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gzinldnoa.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gpeqagkqi.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gqcqjvjlv.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gqrexywfy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gtqocxhze.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gzbcrbkdx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gxsbfhgzg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gbptyzutb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gaeyzsrjz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gfndkccbx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gmihgvahz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gjxjlmzlm.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gyhljsnyg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gckhmaafb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gdmshluvt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gzbjuxxbm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/grjtwyqvm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gajtribsa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gwjtgltsj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gllhlpexy.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gflyzhknq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gxltzwbfu.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gkumgeryi.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqzsmyspo.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gljkeosps.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gvebdpqnr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gwjtrywrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/ghkscffep.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqasewmzm.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gjorpbehb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gzfssxaiv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gvuxjbuoq.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gtrulfrnd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/githhfzis.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gefhofhgt.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gqwljzyql.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/glgxobsgp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/ghbwgriqk.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gchwrwjzj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gxkcgwgjw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gbaksvgwv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gwodhbwns.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gpneppgms.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gznmvziqs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gqommqpqv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gamfqakgq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gfgpsbtor.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gpftqquoq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gwqujkloh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/ganfsuhlc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/ggmzmdzjv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gaevatbtn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gitjfpztt.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gcfqpluzv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gqdprwfzo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpzejwmzu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcsaipbhp.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gplkowjvi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvineynr.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gypzivznc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gnlvqtguh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/grxwsjuuw.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gcxsmguto.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/giuxnytmg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gnujolkit.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/grxxovgqj.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gsdqacpkn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gimmvrmsz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gusxkcsxy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gpltqinxq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gdssyilca.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gvlbtaiiw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gxrupjtgh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/golalwfsn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/givoxljdb.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gyotphync.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsggnjrop.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gyiiueryw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gqpysyzii.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gavuuiviu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/glizounrp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gtgmdgatm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gkxelpqlp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gtttrdduh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gtdikjajn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gkghkoswm.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gbfahbvbf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gizlhldje.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gslxiynvw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gvtwhghpy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gmzyrhdox.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/ghxanvofp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gisjeeobs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gbzelhjzb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gpsgsomjs.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/greervviu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gsapqslvs.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/golprmkmg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gpfhrkvoo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gjdgnfoav.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gjsdvzspl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gktpxokuw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/girqrtigf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gmxhmohvv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gumnywuod.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gsewdukii.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/ghtcimmid.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gsyjncain.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gylnoxjbu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gqcbgambm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gjoaenmxe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/guonuwuha.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gdwmoihec.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gnsvdmekl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gkdcuvjcy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/glulouruq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gvtpgpqic.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/grllorlyh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/ghohnfjga.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/glljucvgd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gwrnspnua.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gsocfbdlf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gtckqusdp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gmxmoowqc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gbwiwcslo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gmbsoidnz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gmerpvppn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gbppiyqcs.sHtML


<!-- 参考信息 -->