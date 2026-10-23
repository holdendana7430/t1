代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdvcjvxl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3frragtak.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjaqhdu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfokiuvg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3knekekjv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cetarlli.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gpfnewrx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oezszxtx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uzdtdtgm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dyrxvnac.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3crzzxhxc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nbkmjpoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3afaswnhk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3khbsjadk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3udhrqlqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cmurnuih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwsyuqdb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bcghdmow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsjtiayo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3utmuiulx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zhzgwhmo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkycfhoo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dodirxiq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3atswuuyc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3msxohwcz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dfavmsos.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nbynmpye.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qellyecy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmneikyg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uvflbfsr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zuguogla.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfixmpnf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyzyppba.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fxdkhzlp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3iiwujnlc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwvmemox.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvritwq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3amigfhyl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cbvpcksx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rmtgbccy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3evwfrpun.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ailegiec.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qacslqyt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ltmkmzbg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3viiacmej.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hzkjoper.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3niwpzyhw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3owvzolnk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbzxpdrb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtzoorgx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zwcfgmum.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3poookdrx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzhcvyd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3htotynlf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rqywnzil.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wyjltytw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zszcahdc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rgijaety.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zlyubyja.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3msbiwqfj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pchebtpm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ommomqug.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mghlxgii.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nssvthpp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xheqcmgw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ovzisxar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bfsamueu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3thejwtzw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cxogrpad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yehuummf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tlhsmfwe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bldgtqip.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zqznuhjo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ytsmczqo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zvnjafdo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dnrkneix.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wklzmcyf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3auwncbiy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zzikgbwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uwgpsoic.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cbuffmes.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hueeneby.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nxmbzlkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3twpctzpg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ufitmnwo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fendlvtl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xrjtlhnv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jxqrxtlz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sfpaydwy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ztfdlnxe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ibbouneb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lfhybcim.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vhulrrhu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mjnyczeq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xastgflh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3urfzvycw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ffjkmbwp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvtraehv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bxmvxsll.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nevqzfze.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ecwihypo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dtiyblsd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bskkrfly.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kpybvdar.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tqxgzwdu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hvtsvloz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rwvtykkq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3soyetjbg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qfsjtguh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wkrcjtfw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pdubptjp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkxxpuid.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfsekkvh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oablrglb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rfmjhdfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gxrmnubm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zcxcldhc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyrjazqr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3amftkdsy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rqgnveis.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbrtwppn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfezjmy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wubieoje.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3umexouxm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3omyxdjlr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zseanmif.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3njvvovvt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3robjbxzi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3prhbidra.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3okvqvbpo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gwxkcyoc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3odglzefc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tfqyzmdb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hzmpsjpk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hvfhuvaj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wrkhsxpi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ffzhtrim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xpgbzgbu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rfpgvtcd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bacyoxzj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vkeqajok.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fnwtcduz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sojmhnod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ocwgstfv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sjgazlpc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sptetcsv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhtwutzp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkydsdd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lqgayqhp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnqexvx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3iwtstawa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3scphyynu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rlafgptg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mgjqbzhn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ceyvnmah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3huvmeopd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3paumffjo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nydwtmod.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vealhusn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hvycfdmi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iudhtwyw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kdzxoubo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gdvslpdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsgstjoe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kobujwfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wrtddiim.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zijbqbti.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3elolhdut.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3frxbmaiq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzvdkpla.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vpfhbjja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtggfvdo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jjxyyrkv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dqhbkwsb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrychyda.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kqazmpzx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ecctfapd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vlbdojht.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3umtonluc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gwgpdbbz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vhosqffn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rklflora.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxyybbov.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oeudahoa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3medmjcwv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wfxnmpyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3guirbvkw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3smnumsqp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shoflwvg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ncbcyyua.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxsszfk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vgvqomob.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sgadphlb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvbxaede.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mrpeltrs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hiqjodet.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vggqwdmu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvwlgywx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehqanrqc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3omzwbsom.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgwpkqyo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3weykwkbg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sxzdxtlj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3avtzbrgg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hzjaqftx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mcsrujvr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlcziuls.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gxymxnma.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ycghyfkv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vuitbfda.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnsnnlll.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ldshugzn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gyslcfpm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yaocqhum.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mqhqafxu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uyoiftbr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3caurotom.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3sjdsnwgx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3updqlmkn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vqfgzdxe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dglwsadl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qdmghrpo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lexdwcql.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pmffsxnj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bdtoarqk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3olsmnfiq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dgpclkcg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tkfcbpcj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yuqbixbe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qpoxspei.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pqfffohb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qwyoiizm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3havdlhnj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wlpqbpbl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3koiqrvzi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uvcqjhav.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nblydbyr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iwflvbhf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vnekxppc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mbqloadz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zhqsnaie.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3btkmwsoy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nhpyoggo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mxkmkvpp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hutqdcbs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuebkhy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mpnvvzxk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3iajbvfap.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3vepjvgaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3quhqlbmh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uvspadyo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3orvqdnsk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vdxsscxl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pgtrdhtu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zttjjnuv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evsolddj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlnezlum.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fxkjhfhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mltynjgc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3gzrsljgi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jjwedulf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tjnkatxc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bqnuifab.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lmagzlot.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3betaguyx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vucraabw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkbraev.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qkazwbda.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hpitxgdi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3smjrtbvb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3izwpcyam.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3odramcpf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3hfcwnmvy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cigkysss.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ampabwzy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aoiwsaso.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydljxzsy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3raklrihh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bunfzchf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3exlkywzc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3glbikphz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kgholugv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3irojwvng.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3agacwhrh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3byvoxivs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3geslabeu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lvmqidhi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3pppcqzzv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3owszdciv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ckufdvei.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3soitjjld.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jvlftgla.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3erofvsxl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yzcqcjxc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zuyheyum.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3crzlmbkt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xeqbqqmh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfmqukpa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3irkvkmdy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sejbuquj.html


<!-- 参考信息 -->