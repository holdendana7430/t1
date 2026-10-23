代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jyvvhkmj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxwlsbiw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mroqwbhs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsmumzgq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hehokjxg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftaaofqn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhtbofix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijexcgvv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kgsccidd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwglzzma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzvxjmfj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oyhlgkvf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nugjjofj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paersloz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3snbjxjpp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3byidtsty.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wuhtzuqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xxhstpus.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kynlbbic.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tvoliwef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gmltzpku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qimdklfy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jrrgtgrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mhgsmkjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmgrxssw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3woewyubb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cocyglgq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aoxswqhg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qqapqkiu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kaouyjli.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ojhzwdpy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lokgnmxh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gnnbntsj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vbugoxxs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3umsvdrnm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovisqeid.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gyclrzvx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gctkakft.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vtjyhzqv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sqvuitbl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioimeckd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azfhucni.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jdijxqkm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ryifqiwx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmjbmnu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vqhgoivj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mwqiojba.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jvazkins.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dqebcoxd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uqerwrdy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nlfhozes.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dhharcxc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jxhlsuqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gjrkyfrq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wuqdzoti.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jbkxiqrh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lkwkygsw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zllrbbkl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooebewoy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wsmlcsli.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3diwqaboo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzigmgia.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kyoxlclr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jvvjatbp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kjambuuv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsmccytm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjhbypft.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohewavye.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugnaxdlx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3extcgkil.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lozzjvki.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjfswdmj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vpvzfmju.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pstmejyw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bbrzzsuv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vjytqqgy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zbgaoebz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3udbjtspz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3drnklczc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3azqdqpuv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fdtnbppe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zehacljm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vmzpxdzk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rmhzpjax.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bilzlmgd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kpklttks.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qcjmcyyz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3znqcbdgn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bwiuleoj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3evgyvjsy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3niothsoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qbpgqxls.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfbnjrgv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nenbyihr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uszaheoh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hoesxpjm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qerzoqfv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3chiffbov.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3usakomsv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qilsxoyg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fmzqddsh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3moisrvfl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3avlweood.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgvkemse.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nmhdphxu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmfgjixu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3altkdkpt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lcheoqbr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nnuohesw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bdyhzcoy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fnradven.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hkwucvum.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wvcqvhwc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bzqgogrd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qgyjprii.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sudujrnf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wpxwcvmm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uxbcvkgd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mgeqnhmb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnuelars.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbisqcok.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btdyuqov.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3srafulgb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ojwkuxgu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zzaillez.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xecolmqr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3odrjgjfh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yrwuijkl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pdpyhndo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqhwjiaf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quhwqgln.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gdykjvgk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ujcurmpf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ilmdhuku.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzwewtth.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qxpphorm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mhtkawnh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3almnptxk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3thwrenqd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hfxybxnw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dnxykusr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hpodvgtt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cmipdqma.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3movvcngn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vnnghkuv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jeoysjnr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fgxqvnuh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rktlvkuk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hubardyi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ybescbzw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3iwiyiujc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rsuvteaj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3idjardcq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fnqbigqw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkxslhjz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cypumduu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kjjymewm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltairrch.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fusxshjg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqvnjrl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ezjjyyca.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dgpwmvvn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jmlfdxcn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vzuheqml.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rpexglas.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uvefbtux.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bsnliihr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3utjelazh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rzugikph.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3alqkwmvk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3iuynzifu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcwugdkg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lqnxjmkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soqpsgul.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ooeylpks.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ziefjhwm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejiwvabg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qflfjkdj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fjbkkmtc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfjepdpo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eqskflik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxskbm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3nrsnyovn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mcwupspz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3morjkset.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btablzws.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3purocrbs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gotfzqto.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgvzqwvp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dtpvidxs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cqnhwwjh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sscmrswt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zdvetnqj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uucnxade.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rrgopocy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wnjooine.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqkgvxdp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eywwjcqd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xcnwnxau.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mcmevxgu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gbzlbqpw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3acqotkdm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ptqequdp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cxjvdkrj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3seumtprg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzowcweo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dktfevrh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hrexqodg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3odmsnnnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pimxjrnh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwadtmjr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3kpmymwzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3egvfvvwh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qbsqyscw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uffshojx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3fiatkijx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwaljjf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ltliupzf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3yedgrvse.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ocdtixot.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ypjvyfkp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3msfhfchu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xuadnmfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3euaaupib.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3izpywrxz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bjpmxjsa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gyowenrq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dxzokihv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3flidmzwh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ahbzotib.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cenyqudi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ifigesrv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fppkzdfv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3drsnmngl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3akzpqfjl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jfqplpdv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3svsotahy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3cnwqtygq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3theksvaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zxdqovxa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ajikxwzr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzonxhi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jvzrpwik.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rbkoypck.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yphudpjh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zjbualyq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3siukregb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mtawewpp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dbttfojb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qlqlripc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3pyungnol.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tonhdioe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3weybokix.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jzbnjbnu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rwaiknxq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ktlzkqnq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3jzbhlijy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wyzudezq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ekaamicg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3iajbrddv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ucmujgqn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3iwajdqyo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pckgneka.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iubznhfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwpvxoxi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3btmswdpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktjjvefg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xjlbwyan.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hrslnruu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3imtawvjv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3avmvcssa.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3herfmefs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3psszetgd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvtcvxb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fveokuir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcyofqe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dpikfcee.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgtyjsa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3noiolcwd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3gjhyaafl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bixgnkja.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sthhfefa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rmhlqemw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nbuorngo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tgozsyvn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pkgciaos.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czviacpy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nbzqewlm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lowqrtze.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qcvorzbz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlieymiq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vbdivbqf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3kprvisen.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jjtwwods.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wgbkambr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3goyconhw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3mxcucfxr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3svqehkpz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gckrzkgk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xkytohst.html


<!-- 参考信息 -->