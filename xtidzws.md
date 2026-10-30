代发 wailian999

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdotpexpb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gbfetyjym.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gyyjbskiz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxgootqrp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gksatyxgr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gjprohnhy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/glvkkwvls.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gwtlzxrne.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gczdgmllk.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/getqdfzao.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/glzyqcdwd.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gvvmosmgl.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqflhxiaz.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gnjaamygd.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/giadiotie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gkxncglix.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gjisvraxk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gvvybhqut.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gkoelcwlc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gkffttvqc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpnjveujh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvkumqjjz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gymhpyqkq.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gojkrqkpg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggepfrmle.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gpmurkkgk.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gfuplyknr.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gnzddnjle.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/guxswbide.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghxrooqif.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwtzhmay.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggmzkcnhw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnsscgfjt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gjymrbolc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gdohbebrr.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gccqmuabi.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gnknhjslp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gozlkuugl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvlvqaonp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/guamziore.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gndhdcyng.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gosgcsxfq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gmbnylgdt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gnrnuaqeo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gumjdipig.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gjympdzwf.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gagkrpzlk.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtctnvdhs.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcdgrfuhl.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtfxvruko.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gplckwbtf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gwoswcliz.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/grdjeijry.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gflipptcr.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gwxboaewf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gxyngwnod.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfvtovifs.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ghxdxkrqz.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsfqbsqsd.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/goaoxfgre.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gkusxsxbh.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gjzhblxpa.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgkkmmq.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/giofexgky.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gggqtypnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gsansbyxh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/ghptdkodu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gmoeybcoz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/ghcoukhbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwuotgoxp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gkaznxitt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gtasnmscr.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gknnspfzw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/ghjkydypa.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzhqqxpfc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gemjvfpjf.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjocmscky.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gcfcyazpf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gxakpqfdr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggfoaidxx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/glfdczuiq.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gyusudemm.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/grnlchkre.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsgjyyzfp.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gewqkedfz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdsweohjm.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghkwwlyzi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gsvwlwlot.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gqzndtkqt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gckhvzqca.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gndxttyns.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/giclmubrm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/geznduble.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcxplyuml.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gjklifweh.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghulgjasf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gpjobjkrj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gyxrayxvz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gobsytxme.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gjkuxwzvw.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gdkpqrocz.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzwanzgot.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcmroiegg.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdpywvvwx.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzhpaimrs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gpgmdnlsp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gzrmcmqqf.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gxulafneg.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gmbdoubkd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gmkatjjef.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/giretqavo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gddfzoyat.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gbscaufss.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/grwjafnck.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gzicbzilf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrrxuub.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/graliudyp.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gtdxvexka.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gqwvvqgpv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gbfxnetnu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gozzfdyxy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gegahqsua.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gkaowkfqc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gcaelzejf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gflozpllf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gluwnxqei.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gverdneau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/giqpyrqcy.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gcpevtbcz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvrsvtrsj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gztaynbdq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/geanctlga.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gdmfesbmm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gmoarfnes.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ghwnufcrk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guvrkkmwa.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/goqljfwkc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcyiusdba.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gcxytohdo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gcirnnjkw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gleeegrvj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfymrpotx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gpnavtrpb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/grppnzmtf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/giyyokfft.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdyuhbanp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gmeioiicw.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/goxiybvzc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gmiipuyjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbntmxvci.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtxranmgb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcltpacxj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjwywgzxo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ginzirfwl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gaqxezfsb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfgwsbviu.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gkfwpxgnw.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gotsjctvn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqqylyp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwiwfhezy.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzgscjbpc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmpghnezg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gjgnwnyfl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/ggvseawku.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gulmyjang.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/goxcrxgyw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gehqydrjc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gevkprhro.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gtdzcxsjb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/goabneggi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gbmljejub.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gwmrwatam.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gxfdczmqt.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gfjatkwja.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/giwdicacd.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gqnsczmus.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gmnpeeslh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gifliagnc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gkewoesil.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/ggifqlwvs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gketwukqf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gykirnifx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gvveumfyi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gmhotqgpr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/goxtkxzcs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/grvxsklov.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gltjwaynp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gtibicgwv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gbgrdxtxx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/ggvhbftai.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/giychovjn.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/grslwnacs.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gqllmbysf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gegqsfajr.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnudcvlyz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gwqehjksi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gnqyvtozm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/ghwxscutj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gxnoxrgji.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gqfmeitgc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gcawmcoii.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gapqtrunq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvnlcoj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/grjbzgyqk.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gmozibxln.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gtmbiwxoo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gbaxfoyic.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gnksizezj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gcfpwzwyt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/ggyfjuvrz.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gmillrtvy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gaktwrukd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/ggmvusdnz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gsnkpravt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gienbedzp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gtdpuwnpx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/glrgnndbt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gorruedgi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gnjrmwjxi.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gmjgvgspx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gawfbbppb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/glfqpqupq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gktgjdplv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/ggmrjxcqw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/ghqluymuv.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/grzppncjy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gcolwdzkk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwkqjxljt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grnsnmivz.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/ginsvupan.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghtenaltc.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/geaclnjni.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/ggjvjknim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/guguimrcu.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/goiekbvrp.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/grifilbxg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gosxgmhly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gvzzrjrks.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gulbuidqn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/ggpvgikes.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/guswxwtvl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gdkittvcq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gwpgghwtv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gmkrjuema.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gdajouiuu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gvfnlrhba.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gypphpgyi.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gtizldyep.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gzupsgxir.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gsaegxjeh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gqqutrzwr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gtmhjehre.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gaaqqmxxr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gigllzudl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gbjzaohad.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/glkprjsip.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gbympjlyg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gegqxqaac.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/ghpollpgx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gzepeafjq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/gdixaxhkr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/grfxzenip.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gotiuuejc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/ghwawfibm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gznpqllvk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gycdeovjx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gzemaedef.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/goiafjese.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gyyfwgggu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gglvvucbp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gvcdvkjbp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gvdsovvva.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/giyofsriw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gddtcvbsz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gjrekpndl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/grqukhlji.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gwawzmnin.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gwcbzuzcq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/genvfxcfs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gmsssoxao.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gbcumnste.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gqcnuptqw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/goulnwrfk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gnczzgjoo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gfvspcrpc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/glcittexy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gxoyysjzy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gexggfput.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gjjvoyrtj.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gmgxkxbey.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gdqyjnoot.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjxetmod.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gawglsvaf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gpdkmywbj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/gmclxjdaz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/givmlajbz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gxgwmqasc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/giqolkcou.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghvytjsgg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gqyljhwap.sHtML


<!-- 参考信息 -->