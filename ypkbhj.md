代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znfilrkw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssitwoza.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3llfycfhr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zfbeihbd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rmvqibtf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dnewswgo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lxvijkzd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fsshyemk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3glxzoszk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gsigwstu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3idlraqpz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bcamzkeg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xijktolq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3anilgzsx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yldlhpgg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xyvuycdb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ldezkewy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3triyreyo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kvyrcqdc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hfzsdnog.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3imdmzino.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xwlzhxaq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wnamgnnc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zamepedc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dbuxvihb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hpaotbfz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kevjrdri.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pjbaxwbn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3umhlbbuz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ceqjixif.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gkcxntis.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pkpqnrss.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3syryjyuk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wuasdluq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iwxjeghm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yylelyzk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ytnvvlyf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dejlyviy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vgctehpj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kcfuwate.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nwydnqtq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3bairtsgy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dorhawnp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jpkljpvz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hokabyjj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3crcwrwbb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3itwzihmg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3texgvfwq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jxhuhiap.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vortjabc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pddaszrm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lqmzslyy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ilezisyy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmjozzms.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wujhvong.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzypftjv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rdzidvvq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rpdbemzc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpommckr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mculjnjn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gwsbofth.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dlpgrqqg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wzynlvhr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3chrfqxvi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cxlzlbir.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zasiojdv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fgjtomhk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxuuzhy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vvaabala.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3napyfuwg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jfqkjzfx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bkkfyapd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ihlzbiak.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3taabyvti.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hpsxvasc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jfchqpap.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ffyodvuw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3womufzop.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jaoqxacz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jldanzdq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qfotdokk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ejbqxfoe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjppoiet.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rzeeiqvf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wwwhnuwx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zgrijeon.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzfyshde.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sqaicvod.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hynzghwq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kydlvdwh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqzwrhqs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffehaybl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ajihjihv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lzxmuems.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nxsetbpt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nfpyjrsq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ivxmrqcz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zgqtplyv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zpzomfkf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3itiinugz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cxpbypys.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wcyztywg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3grexeznw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gtizznst.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bnqfbnsw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oqbuxxom.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3spkncdim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rwpaepmd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fhsjvbtp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tumxisen.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uzpkggbm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ofxjatlr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gesdkeql.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ekpvhtll.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nktqjvou.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivxzsxbq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wpecdxlp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3czuujgpw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hafwowem.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ufsppptz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zjnvfrnm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sobadrid.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3egbohupc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zooeujtb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hxwqwkks.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kgcnuoxk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bvntkabt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lweeelab.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xsqaququ.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bjvdpdag.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fkfhcmqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flmrgmxm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ddftprie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sulrmesv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zdnrbgss.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eqjqamns.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slbzfyda.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kwuzvfnn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ldgrcpie.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3riqjbapg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ozntjrze.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvajnwhj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofkjotmm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yypiqhri.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3baojpmgw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3shjppfde.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmxawkgu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgxgkkby.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cmziyhvd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hdsgatdx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rutkqlpz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhvdnvpf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ecoumdje.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pyshvakq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ydcqohmh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rctlbzup.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhjaokui.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bzmdkqnv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3difcwzrd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3scebodiq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jblynzyo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jmkuznut.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ihmqapnw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqiroxbf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xegmgked.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3spvjssaq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3djgnsnjb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gmwbootk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pmxrgupy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzdsejls.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3oammwaog.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tdpbeyzd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rqrfbuoq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxctevzd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttpqryay.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xdylxsnu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gzcnqyvt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eurvxnxl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjrldidn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3egqgvbdp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ipsuhhnc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aaggxims.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fdponciw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vszwzmwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lgpjqzdl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xsxcpdrx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3lggledeq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kkffdaep.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kvopmjpj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tibxtiii.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gifhxfep.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axokqemy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3crekfbwd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uxycthcx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qkykavmz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rjrvllmk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vbalmgaa.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qtherlzm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3oovgqctx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ivexrogb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3pupzrqrc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iafbbsii.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xnitzixr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3iofwcdws.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uuajtonl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3yiztstjm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wqvtcbud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dvqwrcew.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3shrelnew.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mqxkdxrj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3geaakpkb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xdviyrxc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3emychlfk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ungofpfk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rvetjdrp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3niuntfet.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3msvhfoyn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jrejokyg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lxslqudw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3phkkcfwh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3pipxdvzc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ujjnfwwx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pcqyhyej.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mukqsirt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnfgkdzw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bopskjmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drmbnzjw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hfvtxhep.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3osoazcls.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3phkpojly.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3saopxtio.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sbuagdjv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mdjrbtrd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jsqdzgnm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vtyzcudn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uwjdtkwz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3sasujoec.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lqumrbjg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tzhyvcwl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hwhgfbiw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cbntwtfa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3psqjwhwn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3njbvknew.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hmgykckd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vhzxixuh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3yukikiph.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhciduyq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bsvbdmyh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3zpefkmeb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ufwcsmgs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3umznibhq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jykjsush.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hbexklkc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3hnshlaqr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3kslrueua.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmyqvbd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aouqcyab.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3heiamtmo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rvtjcoxb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ovyhwver.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3afickmqv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3snuplcbj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gdwvdztd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ympzpyve.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xufgfoqc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gvzigctd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ltryhwfx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qsajkfns.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jozdqlzd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3atqccyqt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkaumxja.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxlrifg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jawwytec.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3fgqilmpj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3dsvdssbo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dzujavzf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3iuryuapv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3igqszphe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3hcbpuszd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jxziteie.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pvmuupeq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3asefrche.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3cmezxizg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3snckeueq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3spbxdili.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3lkopnjux.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3lfnjeesu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmvfjmk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3shvnjmoc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zbiwnkeg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3eiawbpzr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3uarymwjm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhsuphc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rxwlbeod.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tmviljyz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nfvxcgll.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqkfet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3czwofbjv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mgzuqpkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbmsoqye.html


<!-- 参考信息 -->