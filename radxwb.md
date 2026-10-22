代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmihunap.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrmdowzg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ecplgxex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzosdiyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yrpgirlk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsovbjen.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcfpotzm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2acntaala.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cixlmsrn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yaslfpik.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uzsugxbi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rvgopzvl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hdfqddti.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lkruyveh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2scmwzzyc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2czzhutam.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cftumuxf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2grkhmdra.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2udfqepoe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2acuerhbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyzoshwo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cqscabav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bytdvbqk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cultleew.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qduzivki.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kqvacosa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ixpdwdua.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2astmzrne.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hfegqcdj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2akctjxft.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmaqrvoj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxsbxjiu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cutsezun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xrtkvyvz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfjmwdpu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oluebugx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2igfwqsay.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dolzsseh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2icwgfdbf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjpzxieo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyoelzbd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2whmagbqw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sedlllei.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jmlscobo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hcebpnxj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xrfdemqd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2inqttoat.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qjijjjir.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jmrzbzvu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfpysa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dmkiqkqs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mqcxusji.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rfufvrcs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blsxwsde.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cqpmbrri.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fkihkhge.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ygnvwzxl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ahwahvww.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bmwceejb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xqnbfeae.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pruskqdy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wwthbtxe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ysvzlpjb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgkibzxc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjlnotih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ecqxkdnk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xqrlyjxp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yysxgmgb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dwsbidmm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sljfgymg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ossqmwkt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjfibyuc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dxntuare.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywxfxhhw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2auxzuxby.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cidzkdru.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kzlwhles.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2takugczl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iwmcfvlv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kehvzmtl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2klhelnsp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ejnpgyfh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rdwdcscc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mowcenny.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ddnllikv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mxskksse.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vmlaeopa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2akfulayv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhoxmfjd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkhjdkhq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tziqumge.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cefuikvj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2knqwdvip.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2otgvdeoj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fonlloel.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bafkpvji.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vgppvbio.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jsckbxws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dvuzipkr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nvxomxsv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zorwzvdx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2frbuvfus.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2axcgbwza.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqhhjizn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gtmbjvlh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2oxyledmd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wyqvmhab.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zvrzejhk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rmftyrly.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2trhkxkxz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvdtul.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2spursfld.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2omydtwrn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wmhijvln.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2izqasacw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvkfnrqh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eawktula.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqfpomk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alsfqchz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dmyjtjni.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2diylxvsz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2stmwcvnf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2peinzfkl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2eycbzicl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sklpndvj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnsmtpmd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyhhzsqx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xswmzybi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eqfixreg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zicbkhzs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjgoqvse.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgvsdrma.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hexomlhj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ltbprpli.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uufdgkjs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tplnxpnq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ogpjqqpt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wxsetprx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xokeofku.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2iscgeaaw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ksgmenhh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mpwlixxl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gxmqllus.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmbdgb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2takcweve.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zndmurvr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cxzoeumv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dqundblo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zeuszkpv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fudvukqg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ooudqbxq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zadkkydp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2shssrqcr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwiwflpy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aspwpwue.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvihehc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fuyhjfid.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2npcdclxg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ylouilwm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lyeulsit.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2erdpkmry.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lbakxehc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gyfuiblx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xnzpmjkc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uddmmlzj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hqjfdpjl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2exlcizqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehxzcmcw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwnmplxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkdlnmpf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2drluawuc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zlhnbwzf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2blxpqvfw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ezmyjapk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ehunfgac.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2uiljwslm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2thtstzal.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xgdlmrzg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pgbuhwlw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jpytfidt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2svbktlef.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2scjtxpnr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cqkqewfy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mncdfvhh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gngcmrqe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pelzhlig.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fkckardd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebxsmfks.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qsrfuebn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kyzzchug.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hcyhtlgl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjwmjtzw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gsnvmsjs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mqrichtd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2andegqjm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tbilbnlv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hqeuirkz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yefgwgzz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gllhstnx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vwjyffyo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eequffhy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nhwmilxe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kejjwazl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bxobpvwu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2duwogxiu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zesnjvsq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2axtrmupg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cbjtnfmv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2erajabff.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcrhpkfi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghpuxhwo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjtwgksz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xgokyvks.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qxlcvppi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lzsptoph.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cqdnzhml.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jvlaxxzu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2adpoytxf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mxgetwmj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lhmtertw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gzwacwoh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zfyyqtou.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2kvmzsokg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ypfspgfw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rwgiuktg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2byzkjbcq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vccrrlvz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qfrvozgf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lkmzepku.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zvcabgcq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bkjsitwv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lihrxydk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxgllwos.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qiqcpiis.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wjrozqva.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dfqxhfem.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2smrgfqin.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyepdci.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2rhioarlw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ijxlvzzr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ppjvbvrh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gpcxasgc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mcvlrzns.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2psboqmhr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dshlifrs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zmlxtonl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jypvbrfh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgbmhw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2eizcadmh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zuwvwitp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2kgasoxqu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2tlrjvqqs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2atzlpdkg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jffxxzkt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pcsxduvf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rtslyqbh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ttlhvimh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2odrviblo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2drwahxdw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hprahred.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdahhlbh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2axtigmxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvppikbe.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pyyjciwg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzyuhlz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vujjcyde.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oevhkzdu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xpniabla.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vtppawzl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dfdlnxhv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dncabwiy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mpkdecpb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2arswyvha.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdlsdyvx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rgmwrhgx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2tyuioxah.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2olpfrgne.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kliqvwen.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkincrvw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fuxtzjvq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nldfcudv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ezpzzuir.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sqlazssu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bmpnljxj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgkvqvbs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2paqguzsv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2brwhyzfy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gdlyuecw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2aevpuheg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2gosggptn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tiscmbvr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lauplyrt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gvuslyxa.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pghoogwl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2niwsqgcx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gnrivnst.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rapsvvix.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xbfmgxij.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vlygyupg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2spdmcfpx.html


<!-- 参考信息 -->