代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mamhpmrf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dausmcds.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ikytukzv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3swdjmish.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eycspmvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pyasqoyj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dzlntyft.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ttddbxmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmayaqtr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yslkcjje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjqctoqw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3alwuzoes.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dmmwslgb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qbdkjdjl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lryjrejy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3txmcqrvz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3kbniykye.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jgnyvzgi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cpaleylr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkycsbwi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbubouoi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3caqfsniv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dwxsrojr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjsffzss.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ummwoypl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahyjrlsw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tshfovpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3knbbzkdb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ocuebjbq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dgrmsthq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vgghozes.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uuvfxdla.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3swzpbzub.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3avxuqfbe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3geespxlt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tbaxgalc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cwzkxfpd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fqxnyaxg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zelvbhmo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pedyinug.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lnajhaxd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoowiibh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nebrroir.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dphqzpyo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kucgihur.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmrbiefd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oakmgbmu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yzsinnoq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gnuglpll.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3efuoychr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3knhlfton.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sksehvke.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yyagtmfz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3skzkfriz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qulkjsac.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3itljibfb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wkyihsyk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fhvulwtn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yuqbnvvp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwcirpe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnhxsltk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jptpqjww.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hzfnktfy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3czsrwofb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3whiobnrt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3elfjotjp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3apeiicsg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qyvmcxac.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bmvzupzl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xqxdkwkt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3asllvhqh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gyouxwyc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3voufgsuq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rwdjyoum.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jevvsgjj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xwuswlst.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpngpbmk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xxxdxybw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rshhpyyl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zonooeol.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fdtqhjse.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uqcgsimk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ytirttmg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kxiwzcgp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qtbbmfgg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lzpjsmmg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tnddrbda.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wgitnxwf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ltytqmst.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cbmbhdyo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cpwrtipj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ssjokisd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rdzzbqow.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3adzxjwdm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ckaptriv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xnpxbwrw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3prartnic.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cxkpvkto.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hkbqtuny.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fuymuuvu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dkdfulkn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zpawhgde.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rwkbkziv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtwzqqqv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myyfvkqd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spajjvtd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqctsqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aeknklez.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gpkrrfan.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvmgrug.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ntrwkyuf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bxyegzpx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avssxuyh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cunjymji.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hvryfxfx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzqnogyz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wilispaj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmbsizgk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xlvhyqpx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fcojarjc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgpadei.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xwptbabj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jklqwxln.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nfiqfrwl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jmdzsrmm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3afxriupi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tolnyhwg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xjkakzis.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kovirwoa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vhtccudl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rympdmgz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kknpjsan.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xfkcuuof.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjxmpmbj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ajxoqffp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jcsjiwaf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3upginenc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ncfmcamp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vguigkmu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jfzuhyxa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bvqbhmlg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3svxurnlq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rybjhbue.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3shilbqna.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3splsydul.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lkdeibyq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gkhohnqx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wxihfuvx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ghroalxj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfrxssik.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cvjrplxa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zkhogrhf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nbanbxhg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nsmyjehb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dbfcfbss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqnwiacq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3idogimsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crcglmyp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ydbrafks.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mizgglmj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbbtrnnt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3thsbeaef.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhjevwdy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zjlfhabf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xtaprdwu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xywnjiwc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3epslwpea.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3phzmwapx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sunuspeg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwqynhcq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aefblfme.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cleiobic.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfkbfdol.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jcubbawq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3blcakuyj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hybnwxmx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eamogaef.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sdennzsd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gygbkomt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ozptrlkg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fxaumfhd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vzpszqjs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfzrlb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uwxzhiro.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eqmxrjhr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3otqgxtqw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fcjrnzht.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dlneimft.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wibqrwpy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3reauocxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3shkctkck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rpllhexk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3toopmdye.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qefdxeog.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vqzvrtaq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3avueuuog.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3heascsxo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3burjkkwe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3paxkxsfb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktqznowq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3koicmukb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3orgqlkvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bgoavyna.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3iuahenns.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xreuxszt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ifrhhbwi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qlwzzhbw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tmrvbecq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxplnco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3igeyoptz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ftnxyamm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jtpvpgrb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dsujwygo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zvffdbbr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qocuzygn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3unixlrph.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rjothsdy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xzjbshtv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yeayzqwp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jtffeces.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vplxfrdv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lxgaszma.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ukasihmn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3uvmidtua.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3jswhpfnh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xmgzzrjl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mmazfczi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3uwsmgzrr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tkkfplwb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3afntpxdv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hyriucwx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zgybgnai.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3swdoiwzv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3awqsyxdp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fphiihaq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qzclzjop.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dnefuurw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bchnpmge.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rsxqzwxy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3buzufctj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3whuftrpu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mzhxjlln.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vqtjhagf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3panpxidg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dpqwibuf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mjbmwykq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tnlaisro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3etdqsuwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqjdebhb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gxejzahk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inmmntfz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3tpakyjum.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lictroag.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3whineknr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ptwlqugo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jmyfihfh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3aanwaoed.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3guctvylc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dhzytlqt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ynwfwzzy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qzfkhuzv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpdjpkl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rjnwvlwn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yvnoebgw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3junnnucj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qjanbvwr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mrfclghr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3loijhixb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ialunwhl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ldkgolbh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3corcjfog.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ulflutje.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kcugnosz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ojqgfred.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qgiubfrr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fiyiyphk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3nzanbstv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3cydobeir.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ocusqdns.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xnnbjuvp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wmmnvbdn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jvkkdjjq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmrpxgn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3omijmijz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ocrgyvfy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3sfnuuwcf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bpklzobi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3sluduiyb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3shhtwley.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzbrxzic.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wgykhcde.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wqksmxpk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3syukpqwm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3djbdjdhz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fatczdlp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qyqanmkf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qbkjqnsh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bbvvxobq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3cnnqneny.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vldkmpis.html


<!-- 参考信息 -->