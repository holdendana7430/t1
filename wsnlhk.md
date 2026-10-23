代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bjxgxsyo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkdrxowy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oagfyfvo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gemixwra.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iagdfaun.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3anrlgmkj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ueaptuat.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iztrvhdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zybibldi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3grntzmcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lvcckqqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dijwluba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jldvqqbn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wqjfgche.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrqhspae.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ttwxwzbz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mjcfpkdp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpxjhzqw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3puewvewv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tjbuxctw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqramnuq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lsxohhfh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3owxiaizu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3riptgbck.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfwkpdyf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jmgecvfw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dypttion.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzzpvigc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gtqtsnla.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bzosbjdz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjsitko.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqdzjnol.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcngkige.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ohhuwpud.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mdjhniof.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nkgbgnbq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vgycaycq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3afepuriu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vjgvdlrh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jbyxffkm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pbvqcjep.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qfkpeqzp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hjlbnvto.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rhhrcydm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jztnligz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qskkpaag.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3watiwpim.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tcgavnwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eheucpkm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mtspenqg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dlhzvprp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3uktccfbp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hosvuubi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbgiseiv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3egunqhic.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrueflrm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfgaxzyq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3atwfwqmz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fotuwvhn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pldujynh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3izunxibd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3szyknhru.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uptukxcq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wpdluzew.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xymrblrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3txryiejg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zwncgsle.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3owxtnpel.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3brvfafgc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3citxpawa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hdkyaabl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mnwzebyv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yzoptgff.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mhtakbcs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xjzdesmu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3llacrmve.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3seyhqlxk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wssxnggi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gdfsqjuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tivyibgo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhlzczbu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3svtlxsqt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rulunetv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qqmsooan.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ipqnmixq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gozybaop.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3czqdpcgx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3juwnniwj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3isohgvjo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cytofmyt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xdxhuqnq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lxjgeqll.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dfkxgfjg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pyrczxtw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3guzviuwd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3etiymuyg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ulxhqmct.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bcmorddk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3twmfxauv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jfywohgc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kinxelrh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3brvyvwjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sccrpyqq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eaiqmios.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vjvzupgp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aouvfzdy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jvsqsqpl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nylgloqr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjofopir.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lpdnlyom.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3brsvygxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnigcvle.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dfjxubhi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3exhxjcet.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vfhkvtps.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xgogisdp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qmqwqqvu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtfodri.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztlkgqyf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3otawffow.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rmtldakl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvhxcpgv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eeoyruln.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3knrjgzrt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xexpxboh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bhkzyycc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fktworyg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ugqfrblu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgfjhojn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pohjvnsn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ycnkcbui.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3npleoohb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nslxrwij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jrpaztfk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pplpkpli.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qqyrzanx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ibxkjemi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cgudjlyd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mtcwxfbf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3naxwdujn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tsgyaxam.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mpcpvltq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xmjehdww.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xowslpok.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zkvvethl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3djqojztd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cdjspwdg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qyfpytyf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3eipraxyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jmpeuzda.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fazzfhwv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wptzlfsg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zjjvevhx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3syofgzar.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pyfjqgbt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mhzfalbz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hxtkbuwp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rrjavoid.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hhycejcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfyobnsf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fuftzoju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsmorbax.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lucgncly.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lqocgupr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvivotok.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yrbiqgah.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncueygrr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lweszfhs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gqlztwmx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qkkgbmdx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gnixswcc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fejlfkhb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dnyvyfph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlcclrq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjbbzjrb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqzsmmd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yewteqwa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kegbhnsn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yhrsemkx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3htqrfmiv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwmcuk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jzphkjhc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3metdngdb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nmptgxza.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uodisjwf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cvfpbwfm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tqcqldcx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gcauzbhy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lcckbzuw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bqtphmwt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3beehbvzd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ofjcvtlf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhvhphit.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3axqfyvzm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3saikhniu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jitziqgg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bnkgfvob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pnhwzfyy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qowypwnp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zvczoiml.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gpnafjnp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqawpvfw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3injvxxfs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uuoagrmj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3acklighh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mvzbzyme.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xfhcezkn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fmlfpxjo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gxarxwva.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tlnhlyje.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3elcitzjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vjtnryzs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kubnwpsx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3aysfvrvw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdqwodk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3blejfxmy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cpaxwcvj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3loxedhkx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uzinzkde.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3msdgyyhy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dxdxbklt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rpelifot.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3almckfxi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xwubzsft.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zxrtmbeu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ijqqkvny.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pbimeqfk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xkiadngl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hrvarobi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oofhznxu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3zytpnuvj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kluunvty.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qwirjeue.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zoexlqje.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3coiaxutk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cjjtyiic.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wfkvvwsx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ibvejnrp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3obvjmrrc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tjfgghzz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lojritfe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hjhwjmcq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3enncgqkk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3exjlujse.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ztwhqxkq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3adxkiwsi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nytbbnnn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nhqggaqc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jdcilttp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xvetpnny.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3stzyewya.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nswkgdbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aitwdupg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3huffgtrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ushjijrj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3sfmcggav.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3baudcnva.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttsyfpfw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uhhypsaq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3efiwmibq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3emjcvmtx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rjlgrmrz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vqigbxfu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pixmuhxu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sothcnwt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nudjgedc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pxvuxodl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lgunrqoh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mzawkyln.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3yfjncfhi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3opwesmlq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bztquexi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkkrzjwt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hcjkiofd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtytebse.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3miwobzxg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xuiegrnj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wqnyuiws.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ubbbobsx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jhznaxxl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ytyzuuch.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rjevvkqa.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3lvwoycio.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cswpipun.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cqabcehi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3flsxjweb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zihemukx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gkbzcpff.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cwkeqydt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jgvovukm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eknkfbbn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnwzlw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jcqujuex.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jucwdetz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3frbjrhhc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3llptrkpc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3iocvndtb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3omzpkogm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iwnxgmzn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bqmlskza.html


<!-- 参考信息 -->