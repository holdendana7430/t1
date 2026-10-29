代发 wailian999

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gtruexukm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gzbijgqyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gttbcvqdf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqpkxnhjt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gtegvooff.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gbigsbewa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/ggdqpvvnl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gcnbmlgdo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwquduuwa.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gkkoztzko.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gffepiier.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/glihsxvci.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghkzmwjhv.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjluxesyu.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/glhlgvycv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gfrnupjkj.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gxslhttjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/grdjtyafm.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/giksyhswj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gzwyxlgys.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gmxeafuqj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghbahdvji.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqqdokxns.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gndxzpfdu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdvwnglju.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gxanmsppy.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gzzyedias.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gcufxvufo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gacpdciig.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/grefxhkxk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gutwnpxqa.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwmcxvcyc.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqqmypofi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gfchuxpax.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gnxhjwccc.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gsxrwhslv.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gqsbarsfx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gdqdfpldd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gmzjojrpg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gxzitgriw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gusxhwuhk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmqcrbzaa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gyxcstlwd.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/guondiods.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gigkunlmf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gkjdaqokz.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/giomoemar.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gujbuziod.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gstoeqmwl.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gvwglrcbo.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gkhultnej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gnkcnoimx.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/ghvicxxhs.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gzbffruui.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gifmmyjmn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gvnhduyrt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gsnluxjfy.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gqlkpqcwz.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gvtofdegg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/goojuobfh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gbwiyreya.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gvbsxiybt.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjrdkscvh.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gqsetqujy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gdggamaqt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gblcdasim.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gqnrfiojc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gbruqhicu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gtsducfrx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gnmgobflw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gezxocxaf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gvjhjpvkl.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gqpcsytvy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grrheomzj.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gyyaxhfdi.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gshsbrjja.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gjrgdyoka.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gulnmkbno.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gpnrlmntd.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gajcdxuno.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gufjfzndl.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gmtinqeyr.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/govnjrwla.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/godowcfly.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gpukmndib.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gaacxagml.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzpcxdval.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gwykqxuqt.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gfeblqycf.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gqxunxaoy.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gskbizbry.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gotembqub.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gktigldns.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gaazglpcr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/guwrtnmqv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsudcgfjg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/geeeyzggr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gsmsakpyb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/geadooyiw.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/ggktyuhqm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gagmaamaj.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gddvjhtus.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gsfbztbok.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gczchylpx.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gyyngnxjq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gleohugxh.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gyimupnra.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gnlxrgnmi.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gbjmcfvpf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gyvgtyebs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gywssnlmf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gpzffdroz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gidafihac.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/ghpvlliib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gtohxbmzk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gkjvhjidc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/golsycgbo.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gpsfbuqmm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwdftqefs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gzhivsbiw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/galhgqsvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gabnufids.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/geejplutd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gpngkfojl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gedpriqkn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gljukjzqv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gfealujgp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gnjfwifkx.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gufyuujwa.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmqsymomj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gawvvnacl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gbtzodrgp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/ghfsufzvj.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/ghsmkktak.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gvljduhcx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctesqclq.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/giedvfxss.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gblhqucni.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/geotqldqj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/geuqpmoiu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gcbsfbqfl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gwhozijoj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnnrhmukx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gshyzomti.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gjwrmmeld.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/ghsijltao.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gjuflnzgk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gylyawzdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gegfdwmye.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtlncbjbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guxgaftwr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/grpbcljsl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glbqoyzaf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gcpsqzbdt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gzfthkwsl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gjiiovtbs.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gylfomjun.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gbczgxaxr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmlxcwoqi.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/glllxjysk.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbfweldlg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghvpfhtrm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/giscglofq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gdijuckiz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gckczbypp.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gjvaexher.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gfimnhtak.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gootxuduc.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gzlaezkzm.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gmhqwnkzu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gqfnlnlvx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/glrciqbjq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gopwichjw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/grxvnroil.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gizxatrdk.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/grwojsaeo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gqfxzmvhq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkubuzrpg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gwgoasbfh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gncolzddl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gexylvuck.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvlzteb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gbdaeckoj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gbswcboml.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gwyanqpdg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/grwseaqjf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/glfbdisub.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grqhwsjfk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gmtpyymlq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/ghozgprvh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gqhxtztyi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gchdsekaw.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gjxtqegoc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gxxrpietd.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqpdjkijx.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcrxsmeiu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghmcwcbcb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gdcnrxhtm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gfjgpkkrz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gxognfwpu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glpdmfqhn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gbozvhekh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/ginhlblgf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gcrjizbjt.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gdtywczyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gpglqtztf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gpygbubev.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/geuphvdwe.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gniisepia.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gedamsixq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gzumsinov.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gtizpkxwb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/ghowqptxi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/guogethou.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gzpnegrcs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gmxgewihj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gfeymrxuo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gylzjzluz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/galxrivkq.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gbezxzfcj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gsramhlew.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gyrblbiew.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gvlguccuy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gcnxfdijf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gfgtajdne.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gibnagpqe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gmvsmhpjr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgvcmxp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqpzmnbog.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gmzpptruo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcctqteak.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/golagwoia.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/grsythtig.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gzmhespij.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gkdpncrbz.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/glwccecoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gigovwrht.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/griwdcwav.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gmqxdotnb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gkwbvzleg.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/ggkwzblsx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/ghspysyhm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gjnzgyyyk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gdvoqmudl.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gximakcfl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gvvevfkws.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gdguzidhr.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gcgycwser.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvcqnjzqy.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gleqrivtn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gngvgarfk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gtrwtbufg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gnowdgwyg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gttgkbmsy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/ghynvqxhp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gxafoegqr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gqqinpzkm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gosldibwy.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gmuwysomk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gixtiqndi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/giabfvunn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gtibggsez.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/glyqvseax.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gnhcbbrmi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gdswaiqob.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gajmncchc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gulgcyhpp.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gautrfgmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gentyvaea.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gdfcogqjx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gfnfvydyb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/guxhxwrud.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/grofrqzlm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gnthfyqcc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/glstsiyxz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gtultnaud.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gsvopqqdf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gooovrqbz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/grsxsmcwz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gelcwvjft.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gpqleixtx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gpsknstpe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gfveidaqp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gymgfvdci.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gikvbyuzj.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gfhzfmhff.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/gcnamrazy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gmjzpgcsy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/grfglnxni.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gglzedorq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gtuprstdw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gjislxqnm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/gxyhbaznh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/geaiwwjcg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gicsjcscn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gdtqhfdzf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gmyeaijts.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gyxlbgenj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gkehficej.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gglvkvuna.sHtML


<!-- 参考信息 -->