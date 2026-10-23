代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zozjkxii.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ldmtdhpf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hayxnamy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nmkidghg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iigmsfcb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3keosqire.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbgkblit.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nohipino.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bxyatehs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaeoqscw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dklnfqna.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3brssaglx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkdyxyju.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3snajrxwa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jkcuwmzo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xeypjwfz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3royinyah.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3sotbiplv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3emoxjnyu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olnaeeug.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvnxnbwg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xmhnpmyf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3giozwhoa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pbukdrov.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vneapank.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hzcupewl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hwfnyezt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nubjtafo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gxznvegn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qmwjcmhw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dynsazwx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3htngyiee.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sdddgolm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3raujrfkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3deacaftb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3emfihmbh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uocyaxfz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuiwddiz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxlkkutu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjpmptna.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3orctbbcs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmpcahqi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dciwnctg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wewphthd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kkwjtszk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cfscdozl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hcsezopd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgkqjaya.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3scjwrtqd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qddadsya.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddkwdvpk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwzsafmf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gedaxdti.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xxypbcws.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rglzdnst.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbvccfjl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qgumzxbc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mlynaatp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3akxhnyga.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hhvsitji.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rkzirdgs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xhjwvhrn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mltghsif.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iunyriil.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qxeboume.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lpnbqbgv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3imyfozva.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xgavnjtc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3oeamqwty.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3msminjuh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3euoorpel.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ddqzvxbq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcrcawad.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlokwrjd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxueaimw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvmrdqrk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pbtfoqug.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kmmzmuvd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdqokbpu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xrbuzocb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ajncvvzh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vzfcjqjp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qdhcdzgg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gqcsjvpz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ikdacqak.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjgiize.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gzyruhqm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3clorsxnk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ifpwndmb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wlhsqics.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vdwvuqvn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3epioepry.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wbmlmemn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vyhshkka.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jkenftcf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hvwnyctf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rrlzehgd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3spuiwfdw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nlncfowy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qdyoyevw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wdzxciqz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3scwclnty.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wwogvqom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ptpumiiu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yxwywgcc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kxymxdkf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ianjango.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hkpebstv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3znphcbcq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ntnuwhyv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ncusirqz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ntqlgvtu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3guynhleu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmuihhel.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3trglyvrs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3obwehepv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmwihfm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3klvcpshe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tiqidnrw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lleasdmb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3srrophbs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3adsndgpg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3htfdodin.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uydjzoik.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rrrlwslw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3iyypaett.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xzbensja.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3noccvldq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hjikjumc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmffsqid.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3aqtntdjg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oukzppma.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rtdyoawe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cjkullqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dehggrte.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3plcvclmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fpddjyaq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iehhclwu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fbwgtywb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kgzkojio.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3oidxohgq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzqqmruc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3aqwlpocr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cmrguyfv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bbsaoitl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jcsnwxmv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pexcvhax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nlytbdry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3niykuoym.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gcdrnwyt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3aspasqya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzfnbaxe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gdeiwmzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvctadvz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tbryejmq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nuybdadp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jneyylgj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hybpbycg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtushdra.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hyqqxnjh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3irelfgqo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfmxumte.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mtcwuqqv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gczymbtq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bhzxslqw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oypptnsw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3spsgoxap.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtbbfpb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3poakwabq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3edbfxazy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wwieogmt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3phlhopsx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nebknbzy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3csuvnoxc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3splsgjkh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3klebkzxy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3whcwpwwj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qwtrdviq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uldrbdag.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3itezgohu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dkejxgpb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3apikiyjf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3omervjsd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xaxixytf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kganjdnf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmyuiesn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3luymomhi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3flrspnyi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3cqbhudzg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3otekafep.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nohqibak.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zzwxchgh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jgoyaohz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uymnnofg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3icqvpsrc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dloizpxy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfohyub.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iouytlki.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3scjnzatd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lsmuxfpq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kapfuscg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ughcxwcv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uuoihqmo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zcibdgsu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gwoxxwms.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3getrhiib.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hyvmamot.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vrmnbrrf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3repdvttf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nmifepjf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lecagboa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yougamhb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ambzsrqi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mbgqtnkz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tgdsitiy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ajjvpzns.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rvldthqt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3aytbzkuy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qkcnmzso.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3wgilyzyx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3qwmyxmqk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kwlovqlj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jiwcrwlo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3uhheinsl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wqjcdksh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wffurdcj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xpbagbzb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ajktfmxo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3atwjrtvv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3huthapvf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uubwncem.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tasernhu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zzwnhndf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pgqvrmvt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3aomvuyxb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fsmrgxcq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tthldwuf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3htlpgcrb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mtffgxtf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hyxkceae.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3arzevynq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pbipswva.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rxhgchqw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3guqhqbro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqrnmeqp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uszvnjhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phdayuub.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qxteegjf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ltctsmsl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ofelxoec.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zqyphgko.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhgfsyw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ibfincyl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ymijfgxo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fizvejpt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3svzukwqg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gqnvqjbk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zzvdtgnv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pucpiqmi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3qglrlxqb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ywkuboje.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zsssofkd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hqqtxgdv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vlshvtbe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtrabtqz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3twtalyya.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtkupoy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oopjuifg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3zdpvnyrw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yfofxfsx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nyratbfz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dkreziwq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ngsflbqk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rrawslqg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hwyphgwn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rzimturk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3arbjsjow.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vsecaqeb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vcqcjiuv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qjwyraxk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wstxyhul.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cbglcevq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ubpqzsyb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3deqjtrat.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mafjlehn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gzutuhkf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3amjsfcqi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sviaqdtf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ponyxciw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sgekusjb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kyrfybsp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3yvgdcsgl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3frnzdwpc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dspckkfd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhuawl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dsoykwif.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fwfenmzh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dqvcgbty.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3jodhdrxq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jzmbjxia.html


<!-- 参考信息 -->