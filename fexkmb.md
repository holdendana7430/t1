代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxhgqesz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngdjnqeh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwdbbugv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oiozxqct.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cudatrpq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhaootmx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dkprrwwe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yalssznf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vfawgijh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tgeqvfck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oleqqaid.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2makgoqio.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ndpxuhas.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2aaoachip.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hzvkdpew.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bpyumrjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2grhdesio.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qfsdabge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bztqkltw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tyzfvglc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bnjiqvoh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zyxrvgsr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oiwcyclu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2iczisiti.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fvgqqvqx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ihjpswyn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2smqntdnn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqcwjsna.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tamcxwuw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ypcnrsal.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vniixcmh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2llpssjgx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nihlprls.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2serkjfhs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uybvgqku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pgxfqqrz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jmjpqjth.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hxjeaprz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aglmtmbi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aoadiush.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfxeizke.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jnnmilmn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pddxvjnm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2finfqssv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2reinybcp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2seehhvxr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ljnmtgcr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xavelghb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfveyhtw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyqqhwd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhswuowt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqzjosal.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kltlnkxn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsnveaze.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fdnnkgdk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ikxpjnht.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jtyaxpng.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzifnaaq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cerentyf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvykcpsh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eggpgafh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2alxjpsdj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bqzahwnd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yofjogbj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hmoqdhfc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2huhmnxco.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thqufcym.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2klmdlpwd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elwxwdrg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ucafldvp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nyenqriw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2epswolqy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gtwhdkxd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2uvbwdwhv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bzxxpihp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejpuvwcz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgvvnn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qbathmxz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eapkixkm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2egaxegwu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wivndbtd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2puhkkeph.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hqzexaic.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uekmiowb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wspfzeyx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2grjxlldr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nerkdqwg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2llnbpxzf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dpbzbfjf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bbmzssft.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tsacplte.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sxivonok.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bnwrlhwn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjwripjf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zflezeuv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tvegurpv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zrhpczme.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qzldrojq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2smmohqtu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yearwlxe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nbzrpgkt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qtwspvuk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gebhdmer.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uxmxqojn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nimpynwb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vwcazxrd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lxoscnnn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iuoofdac.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ogtvynfr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lzezhovb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rsgtfcvz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lesyrzgg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pjrznveo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ioarfwhb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkatdkeh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ixwlmczp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ygbzbyvn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoyuizvu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ulynesrh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ilzwrqov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzrfprxa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhxkkdhc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmmvudmn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2girymqyk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lmapwtvs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ietokkgy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hgyhfgbj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2armsfttj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nvlsytsy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hneonzgc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gkiywtyb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fyqgepev.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lsifunrl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ltjfiedf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdlvfqn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wazxlaob.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vacgmuuj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2whlcjgxu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vptorwga.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gsatthsn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2afebeazp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwrgaork.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ycohpcau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zpdlwysk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2axdbkynm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kxijplul.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxogtpmx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vlhmdtpv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vwkqkvgb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2avzfoxwr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ygezvbak.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rouyhinn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tznwocek.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ygjdrmpw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wcpqlhpg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yilowbfz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hotpbjeb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2slregrxa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2okxfmrbl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xehlvwyr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yihxebkg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2syqmqjnc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fglftrdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtejqpeo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2aylbctae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gaaiwsie.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ohkmgpwy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ydpkxdpw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lofainle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxkfurq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2voqxhrce.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zbxlcayj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wgleaxrl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qddzmufo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fkvsgclk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cqzvgnxs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dxuwfzaz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkxmwyg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mswkwefn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmjnzv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvqbdwsw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vixjelvz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mnomymcs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhiyjovu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dsbxvtpw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qipbetbb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ikrpvyjj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gvfvsyaz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jgsekikt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ukccrlmj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nqpamhsn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fnchqxgk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vtkcxkrv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zzgyqery.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gbfyhvug.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ruarveie.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vfmelcxg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpuhlnmw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ylyfmyog.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fkjovqqq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2puaqxfiw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lgoiuatj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ztnvssxq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bnarbmaf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilodypdi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnegxbwa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mikdllef.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kunfqbzn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dkvwsvnx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ohsjxjrv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xevulusv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lqwumjrt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jqdzuzzv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xtdcgpzl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2evjlemrl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bfpapwxs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrzsywc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nxqsxamb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2sbfcalry.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mlazsuhr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mtdgvkzn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pghgedzr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jzrxodch.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gnanfsrj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yhjrrsjq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2lulbfeiy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vlbiftek.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yvqzwsla.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gmjtpuoe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qqlggeih.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ulzxqunu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wikuyjlk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wwmgqxdj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jqhhbgrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lmnbannf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nxdessgp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gyjnljtd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jmghrcrx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iumkhvlr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hyczjgoh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wliclvfs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vtdntyga.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ssexokaw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxsfstoc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sqlnfhgu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gizvmygy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2bgdrubna.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mxywoxpk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lisvkkxm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ekkrusnf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tbslyiad.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2iyzxurqd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jkydgwmv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wlvcxzrr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2txjlmrag.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqqdznug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mribsysg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mepsceql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykjcxlpe.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nzixczhk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhthajs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2efqnaeoo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eghalnqe.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdknrxzf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yspyyiqx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmfibkq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uvrbjwbn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2effbbjrt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2iomrumcm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oipculvq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eziwapja.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wrkajvjj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lwkudats.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2klddochj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xyfnodzz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2erybtabe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkvcphyc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ameqpdmu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvcxlj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lqsnvkft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jfaewfhl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmocfn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2wyzdqaox.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2bfimubyu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cywvhths.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jbxtqmyw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aogdpjnz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnvfgfu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zvtjzbmf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tjrergqb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2mkovooao.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2opqsnowv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tjwqdqhp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uilxakmf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tlipkggt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aziizowq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2woaewbdm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdydyagm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dcnetvfm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjxkpt.html


<!-- 参考信息 -->