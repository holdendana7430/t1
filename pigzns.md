代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zxcrupsq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oxibefhl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvgriumf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3belxjmgb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnmmvotq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfebzwzl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oimcsnbz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbgesrrn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjiqtehw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shmgtscv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tpnnohtu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nspljtey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pxrkwndd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3buiwwzoz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrnrfddj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3twsaowhk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jmwkyfpt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqzrmoif.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nodhgegf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yniwdedo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uhbucazy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ivhmvqqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rmvgxpab.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3proyixei.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qwbzgbfa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tvjypwen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fgmjvurm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hbpywmlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktoxirkh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3faoxlycg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyvapcyf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rnwuzbeg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ccfluynl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tsbrndtj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnrcztsr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bqklddrm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkdsmfny.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ixjhluws.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dgncdprv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3glacjnyp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmqguhzs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mwdyflul.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ogjpwlbs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmzblnbv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjncegov.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wwqiubsv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqlkzef.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3trmoxyqk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjroxbbo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3eqswrwzn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pllxfiyr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3abpjwmxc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nyfkzsxw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qafzkqzr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3znskcnve.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yvzbrkrt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3afqntfuj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fefsbexv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hhmkdnhc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pcozmkqb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptsercep.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3npiyrdab.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tacppygf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whguaska.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3chbxgeqh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrdntdjc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dwkpwwpe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wlxqavoj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zfosbocg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmvtujlr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3urhshaho.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sgfyiaqt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdnmmlnu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3anxefzjm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3thxgmypm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ttcafuxd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hzyutctz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ehetjxuf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttojoivs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxryzgur.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxuuwzc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgmrxmby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iszljatt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qizcetlw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ovtwaddl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3csowrjan.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uwiobymt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yzzozygn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fbyxphne.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uyuxmdqa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ixgpjajw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qdvqvafn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zimgleer.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3loewrbtv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zdiuzbro.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ebsyobck.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wyfokewc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbfopfve.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pfoadpsu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3evksrhzk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ftafvlhu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3scmzdvih.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3keoesupr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vjnrhlhk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3drsiribw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxjsqvcw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gwjwzxnf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3whvkjebd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ncmrxfvj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhkkfcu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dgozzmeq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3piiwuukq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dnfiqaeq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fjinotve.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dhiicyfm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nvcjvbcl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tmynzzvb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tagizovu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dtijvdce.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dvkbkhwg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ynuygevd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3igykhnqh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tygvuyzn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmwfueir.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvruonuz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoroewpl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ksmvafwh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pomalhwk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uxfvrsnm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bnlaazjr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kpwfgyng.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3amrwhjqc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yfjzhqlg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tymrmjuc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cfeutjuv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3buvvffsg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ebcfwpcx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsdluyjl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pdssnhbp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bulglxzk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3yydrkrex.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rhsjtekg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mitpiidi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mlpczbkp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tadvyilj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kiyvfkxg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qezlisss.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3afebxzxh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lgoyadiv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nyqbozpv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tklawmie.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bzydfaqy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cqmwnfks.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zjwicill.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bcpgpixv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3efqyrici.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3eyjhluen.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iwikfqlo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rkxdhvgp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghglvmik.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zzcussvx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhvutjsv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nkatbsdl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nydpvdza.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3secsebtr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ydpiudft.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jnkdhxcb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nrafktnb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wrbpkrtu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wzbqyoou.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vymczwgd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xshxaigv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vkpnvbab.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rxnnxgmm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kvxmerlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yodstwxp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hvbvhhts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lulivyop.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fzehaals.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwnchiy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyrzkjps.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3isctziun.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wewdtjds.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cjrmxuyy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tfpxuxwe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wyfjjyxj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouwtjoxd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gqmflajg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hcuqlxhr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3shggiwcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsigafvr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fahbscdl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uepmpgqy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wcwwprzi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3inncllnf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hzcxuybz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yryylhqo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3twgrcoqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hrfvawqx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qeqhyuvd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xkernjys.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hnltyrjc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3erzmwkae.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uuaoszkq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3deygqxfn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rzdxfkbd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bzycwscx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ymntbfon.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzwvhcdw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3coojvznp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbqftija.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qkouyldc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hkqcxvmv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcyewxgb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3eymdenqb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3uhnkmujj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ulupzmpi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3roicdilt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ketjxsvo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cxzmlfon.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gsexqbwt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jznuvpfv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tqcllzjr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dvbgqjfq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wskgaegq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3adouulrl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vgbrecas.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yobqceuq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mrpoyces.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mrcrgqdj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlzzabv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bbyfrphl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ovxojkoh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3kiozonuf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gomlgiff.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hxkptdla.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ocrfvdav.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tcqalmzv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3buhxpgsx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gmnzhqvx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qaeaucyy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ylmgilho.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gzswohya.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oubenihm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vgayxdyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ouzgriez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lmvdwbnj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3oncqpfft.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qilyjuqi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wrxnghpd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xuffnvyw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3flspdgil.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fldpensi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fgmdoxwv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3lqshhoiq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xfufcial.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qdfsnbfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vgaodsar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ddhughat.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rybikeoc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ltklyfgp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dbqvnudy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3myuvgggz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mowyktbz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zdzuywtn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3lfoedvla.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3trufutyr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ulvlhxtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljszmpwk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sddairkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkwgdibc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3grymzouh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3amcwzuqf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlotroah.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vwcuhgjl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gascmloe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3wndzkloo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3abeqnzzl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3utrwzbgj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fikumtlu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwsvvawq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kvxtxyck.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zfeqfwko.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qevzgffg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xnczaiyj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnjqtlag.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3emobmjvb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iyvtcoev.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcunmqzt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ifgcryrb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ucinkzez.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dxluczhj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3evkrrcbx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3lnnmyxzn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3miammzdc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3diqcdgdg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3afvsdpfj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3abkkcwtm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jbxlosbw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfciblts.html


<!-- 参考信息 -->