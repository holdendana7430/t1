代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nqewubgv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bivfddty.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3criezgyj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bwbncfdr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tiseipkv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xagzefyl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mnruuqta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nnkdkvis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qulnbsvc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kywngxnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkywdbcs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jmyteqra.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zkuwhgbi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kymemqlp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3emncctnf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3becbozrr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gidsiyuw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rkdwujig.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dhxgaqdv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ibsfpuoo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xlfvfjyj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xmxlbbex.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sffejtso.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wdmdhzkm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twxrmkpu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lmpctzza.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zcfzuqes.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdugvwqb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frmpxhsr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mhrfurwo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wgeiuvzc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wdgqhkkl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpokgo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kggnyfkn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qejmdglm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qkltwrxq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3odyjnrsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zrxoeank.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ozitclzp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mibjjiuh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzzsjiaj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cexgvrag.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3apofspef.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3layvwmet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3chjsxipb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jgplgaer.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vtyzokjg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vqaitapa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3psvaofmi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oexfjbtr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3njlzutbt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oehgdyqv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3npxkymuo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oevsaydb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ijsmvybn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehpnkqko.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ftwocing.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fctvfyff.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndslvmhd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mwuxsdbw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmiscdco.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tironxga.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mmtmcpic.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xlgogvvb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vxrnholz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ypsdgpfk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wvorqnjp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sooseycu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ojdrddmi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ksulenoh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fylqetuj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uphrdycx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qnhvkjcw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zqottmjy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mqqkvjim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3maeiqfpu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqyaiphg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nkpzfqse.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3horzviup.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zchjswod.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tdmzckqy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3txhefgwi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pbjsndto.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zwrsgjzb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3utizojph.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjhdlpll.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xzbcwjrk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3msuclpbn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urzdufxo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtlhvozx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ofoxeaxj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3omzoclmf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dukupzax.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3amobcmvc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3exvrxwgp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ketthvix.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3igkdzayp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ccyynjrn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fvcsckka.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pnwvtbnu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nmextjmi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rpbzsouq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wwmchimm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olioklsh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vmobuufq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tturcacd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaqpruap.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hlklfdap.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jexqgnuy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kpfczodu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fgoaubsu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kjnplegn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhxwir.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykupivdh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jxmprbrl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3orwxacvh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xjsiosxd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iijuaadh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zmcwqmuv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nswkffjo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3knictjjy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jchztbrb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjkusnxi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fbasyqqd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmyect.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mbgdpjrk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ausjlhhq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3olvjatwq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cdtqcpvj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ovezducz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hsiqrvsw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3opxfngac.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cqrjdzhp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bripwolv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3twcbpllv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uacgfxbn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wqxptaaw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jaxeipuo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rqqlczsg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajtjbtbj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3isivoqcx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gioixuog.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rfomqjcx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3aryhayqj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lwbffgwj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vulfiqla.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wniikamw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mbbpkqbo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wexsiuop.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fgfbbhzo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gaampqvi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cnrhkzuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lgexdgjj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3urfinrsa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3difyizul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftozjcmq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wmuahmos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzcjvfft.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3netvntlb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eqgsunql.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3padbjrog.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3okgsncrj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eybcsrqb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhtjndb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3sfqkhoty.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3atxdefrz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ncnuiqyh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qpjbhtfs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kpupdvdr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvalfete.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pzbvpkuf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzzlvpkr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdefuwln.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ogebwdvu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikhiyskp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ezxanbdg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bhbpgtju.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jnpssrvk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xrnhnxsq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kijmzgwl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ulywhelf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mntmfgaj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gumhorxo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3osqqlfxi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wkixgwzh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwiaetgj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3avivqvqh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3birkgxim.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylrqjrdi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kclbmvcp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcazuvfw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3eesjbhgx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mljkjdkq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jowwdeow.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bapjzbnm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cheonzkq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wyvjtfxr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xxzcadzx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3stmmuunt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbjiwbhl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3onzztqzw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3frflpbuo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfdruumc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rnrphfqr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3igbwodvh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wsbwpolu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ofbvphkt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rqbrjjms.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3eqogpmgx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ooftfnai.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjsgacms.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3idqmtztb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3veaojyut.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3palzikht.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cabibntn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zhkndlxt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vdoymakj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cvonaeac.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fjvdjkuv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ljaseugb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vrvlhful.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kvrudsqg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kfodtgop.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3sibbkesq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3udlxtmry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bweqcmar.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zsiylkxe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kcbvclmq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jyossaac.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jslfztdl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3txayjuyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jdmuljvp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qetodphx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3seldaalm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ndskmuzt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kmcelkud.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tuersukm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cygftmga.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fiitcbub.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rzvqfroz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3rotunvvn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qnbuukxx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gcqwkgpj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yxoazkfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3boepkxky.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kmyjjbpv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3biemizxw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owwdtuii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfmcixnd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rupfxoqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jykimswx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yecnxgjz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pvrbntrj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3czyofedj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hkmdaopl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hydudgye.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qexhtdtx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xyqypjyo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vndchsei.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tzrlaxpd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zpwvllue.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xpmzgsdr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rubgqmvl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3phbkjwcj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3oqufpkyj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ssmgkosu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3agrsbobj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pnxhdspb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fatofenl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bxwzwuiy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxivfxnr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cztrdsqw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cyttkhzz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3yzfidsmz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hnymmdpy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vgtvasyu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pssthmpk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3vgaueico.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3apaitjem.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdaugzl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3litohvgg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dayrnooq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3inmsislm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lblvksmn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ipfxxxtz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvebnju.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3oqvcpjpz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vpekotxg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fqvbtgsj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qftbswch.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kraiyzzl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3otjdgxjd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3noujglih.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jhrjdjsh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3llrokepq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ejypkkrj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ndjmiyxz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fyqwtwdo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ybslsgvy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cbbeemql.html


<!-- 参考信息 -->