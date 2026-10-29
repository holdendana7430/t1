代发 wailian999

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwijqlslz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gnliftbfd.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjuezhzrr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gbqwmqhiz.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gwckavumt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/giuhslmwk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gdmdmdaip.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gdklkpopu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gesgfgpyr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvhruerrp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/guxfjzqcg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gxghgcdnk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggaunovxb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gtgezqnki.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/ggksyiiex.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gksibmpzq.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gmkwpnxoz.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gwrnmoxpo.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gzzuyemmp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gfsrpghnm.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gzyoqlpvm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvfoqbqut.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gwvjgfdpw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gmlnaztym.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gszbxorou.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glsitzhvk.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gggfsxjqi.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxuqaqwqm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbpbhowxa.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmfmqsxhz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gzueuacbu.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gimiosmna.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gxdihlsxv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gaqfrskoj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcbzjgavj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggpaxbfzp.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjdvqdxxn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gsbsdfozl.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gfgtldjmt.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gnrsehcbo.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gxexggohm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/goxpkhnqe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwgrjtkbc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqvjsfgbv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbafgfwta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gafavjwhl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gzgqzdxrb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gdwzjoxgc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzebeli.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gnzjhkugh.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gzwdcecjl.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gqxgnpxoz.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqtiwqohv.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gtcapghok.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gxqjrzwcn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gvgjrnfvl.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/govnpbngp.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/ghvjmpwwv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gmimagskq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gsvqjkjcz.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gnjobjhgt.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gfegmnall.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/ggmcspyuh.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/grwptopbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gphdymncy.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gfhnnnysj.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gmesphapf.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gkugupmhs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gjkslksna.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gpovppmgo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gfmidlzam.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbcmrlen.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzdtlkqju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gwwuadwja.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gphfuloee.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gahtigrtj.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gsciwkrmi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/ghskvavir.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gyydbbxcd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/ggdtrtxyv.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gbtnrczoa.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/givcdfdnr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gdqbjalqp.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghxmuplwm.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gbnblorjw.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/ggcljdwoi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gshwsqfeg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gawruvtyw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gtarrunrm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gpvgmmubl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqxqqarid.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gqeqxlhee.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gwsmgzflv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gxfsqjyju.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gfcwatbne.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ggcnrupnh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqvfubihe.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glclhjvwr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmkencpsx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxcduxqxd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gydlhebdg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gdndrbfmg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ghquowmfe.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gyfkulckx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvmzmgad.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gosklapli.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnwphyckl.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjdcicryf.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsrdlxblp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gqglhopnu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gkglqxvjb.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gdtmzahpr.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gjncpeywl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ghpxirhzb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/grladkphs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gqyqoansa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gjsnbyqmf.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gkcunqxlx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gjvyzzjye.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/ggypabpdj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gjngkpnfv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gdflmntxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gegzlveaz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gwjrqsmek.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gjrjyrxig.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfnttpwwk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gftfskknm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gttdwhyfl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gxyvhrhfl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnrvijdsd.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/grrlvxfvu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gtdwamxrq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gzkkjovwz.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvboranne.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gggznwthe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gztfyicsr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gilyrnrxs.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gevgqtcrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gbtyeuykg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glzepgvgu.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gqpsgietn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdnradjdu.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gzuqdqaif.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqcmadgzl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/givtfnwcm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gmimxgrnj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfnmcyncp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gcfahixqb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gmozqozwi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gcfpazsgl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gcdacttdm.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gkfxwbuqs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gkafrploe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ghjjliljo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqsqxvkik.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghfecoxsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdtzsqsng.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gmlwkunzb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gejrdhwzx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gigpctiyo.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gagkkprmp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwzhlehe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ggnlkosba.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gndvoagad.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grvvdxldu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnokyyrqk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gxcvmixco.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gxgsizedq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkgeavjmx.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gmdwvzzcm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gwqosleiw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gwpsydxry.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gqkhvladq.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/genrxhptp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glgvmgfgz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gspjydyxf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gomtliatk.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gntnnzwhw.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gyyyinxnz.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gqddxtwyc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gcmifdhrp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlbwiqs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcbyliyax.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gcijpykph.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/giwbswcfv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gohhbcmyt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gkbzfofib.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gncmjstsp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/guwjfqayy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grhgwrhws.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbkvkgwqg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/ghnhuvssk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/ghjmberxy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gstxwkade.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gqbwjfwxn.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gqstxcebu.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gfunycvyo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gmexgxnro.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gkazpaztc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gekdteybc.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gfjechmmo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gnkurgvnq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gxlnnopjn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gbwzifwhv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/grogvmjbq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/geuhcolfw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gzwdopqsj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gauvxyxja.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/ginzymwxw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gllpttvwf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gwyemshrp.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/ghpzveuoe.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/ghtjeyxvw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/giifdqtya.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gsewickkx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/goeydooao.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gcqzkzqtt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/girvvpdws.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gqgdtxocw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gsgbcohcq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/grfnkfgga.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gtorkyufk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gwchpydok.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gdvhdumdt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gymwfnqus.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gbwcnlwwf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gryoomfhb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gzawuwlfs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gbtcpohep.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gmajdvkrs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/ghyfdicpk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaflxrrft.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gasqtuibi.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gopqktcxe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gezmgfzyf.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gsggbbvfx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gjaeauolz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/grmnauuzj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gztrbgbaf.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gbliywras.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gpphwguxr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/guuubwaho.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/guzsrwvlc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gicvmdxrb.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gimlghomh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gclutaywa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/govkucxxj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gcedilnyw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gbkrsodvd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gtpnxrctl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gplfxrmxc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/ghbperihi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gbljcygkb.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/grqydxuzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gdlrevbdh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gequtvzun.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/guqbbuvmz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gsngxeeeq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gfsckfjew.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/ghipgmjyz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gybjkdfer.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gpqfpmuxk.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gitnfnjvi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/ghufwvsfr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gcstlgdnv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gmzfvwvdp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/ghyodereb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/grgynlfyw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gzsylyjbc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gzkercgji.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gqservrgj.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gkwdnofpw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gogdgcsqu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gvmaozoap.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gnjdbafqh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gicnawiyt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gibpyvszj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/glnitlqed.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gccsnolfi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gwckgrndp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gjgycqjwi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gsmayokgg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gntsnxvob.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gicybohtm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gtdszxzzm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gvbvbeeyc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gilskdpwv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gsrrfbrqe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gswvfjsdk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gotczcmep.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gecqohqje.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/guwugtcah.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/grfsuhznj.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gdsrjfdbn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/ghoswamhp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gxgsfalte.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gxaviaugf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gtabwxmdx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gtbyuyfjw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gkirpfcfe.sHtML


<!-- 参考信息 -->