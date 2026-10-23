代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rckobfva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnexjfsj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtjyoqya.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwaslqgu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ldqnmppt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdhqnotw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qarkuzpk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nxqsauog.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yvimsgto.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3sjfmduop.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qlifiggn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uyblfedy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lflkgvsa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cwrnpubx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ufvwurar.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dwervvzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzgllyxj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oxlpzkrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpuiluqr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aqwxzgtl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mjrjxlsw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlojhzlg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bwtnkhpi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjxbhlvd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zufutuxq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ipdsdatk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ssvfgtmk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ndjyxhqn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pwfjgfhe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jhsvhane.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ucgzdfkm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyockpc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cuzftvar.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjoqbbqv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ksmgkjrr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pngjvtim.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hadngbyg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qeqhsuse.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pmzjpczq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vbwurzpo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nzangvly.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zkdflyzq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uvgkkbod.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qwomfjpc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hoyttrmk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vlvucewe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yhrsikza.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hisfeuzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hlmqvlcd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukfjnwop.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iuhynezz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnsuhhq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hztohgya.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tnbkyyfr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3orwtinsb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wipdhoiq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ltufymhs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkgwlzdn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gtzhghdu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pgptzouk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xzqkktck.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3szceuojn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mgmhnuip.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqhdkmcd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mmimfkvh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rhemrvmi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vvmqngdt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xjxsvcjb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbeoffrp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uugfisrk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lmfggthl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppxuaymf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zewpxbai.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rzdcciam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kypfpqzf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oihmjyiu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wthmwubk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dhekcouq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tlhvxvcm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ojxpmudc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fpchdqos.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iysormsk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bjlalyyu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zuqomwtu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cytjyoco.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eekbrdnu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqlgcc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bkuyyxme.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fguahhkc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmvjrpyf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ihsthzgf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mddtphof.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cvcboykk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fxgbxhdu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mvzfgweq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tniclolh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rymxited.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdcnpjjr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gcigziak.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ymrrejqv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eykmesgu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kbakxwgy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gbmtfhdg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bnkaaqgh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3skupxezr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3drhxzfjc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oszerinz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nvpnfxea.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uxwapvls.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3oyueodgv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3clvjvohj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhfulyyr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nmbfgbmf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxcssfve.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctnpbnkq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3frxjezkr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nmvxyfhv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeifhvqp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wauqfviz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hrppeinp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjhcbbla.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3afqqlsgh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3upsmktrm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mixtwehm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bsqzsuch.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxdbzdvn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3llupftza.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lhpyjhci.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ymjxovvm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mjnlxsxz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vhykczxg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tojaoxfm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3knkrlsmz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lbkfnouf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uizndgmi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oissasyz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mkkxvqeo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tptgizca.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3guolzgoc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3speaemfp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bctodxkt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nqdhnmbz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3invucgbr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ajdewbir.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3suzsyfgk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yadaeikb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnrvsj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvcmuurd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3prtpejpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mlhojpec.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rdigbrwd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbufxga.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vuqcxjqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtkunzl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pzbsazic.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wehmnpia.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3aflfnhkc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3msdsvbcf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3manrorjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3awqppfzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mzbhbqws.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3evccintn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ppemjstf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqgpkfkd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vgtdklup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3galzbmrg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pjvlngeg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ruxpwkdy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nyrnxofw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3swfiqsrm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ycrdfqen.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qlxrvklv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qvyhsiuy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qccdellq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnbnoaef.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bkwgaqst.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nidaysxb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xjlsqwqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekdavrah.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpehrsft.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rdkwcasc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3teguaxqu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eftkpqki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vcquwqdt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nuiizitv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oplgkjtb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3giwqjekv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aejqrnrz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ygkbsdnx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hdziyqss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hpdvpdgk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uxcwpksg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obqqeevh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3oyxkifza.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oiuwjahg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnyjqukp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yocxhpch.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3crxuyuqm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eqficulz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wwddzqrr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3evezevjt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkgsudrt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3okuvhbai.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vpfeavft.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wfjfumkr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hvabnzii.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3riuqjufc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ovaeuurm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jfceqxce.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fvabogax.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tttfhpkf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ikdqysfi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3athplmvi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bkwvgbgf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rntknqhc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ukdbvxzf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cbfmeynq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3orxsiwxt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xziabxpw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3edpbfarq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fouuulun.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fexdeijc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3alqoagch.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdgtlovx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yrvqfpyp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fdwhorgc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ftvgmksi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tvtoaujb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zutfpzpn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mvdvbzjt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3kzfiloho.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3sjjdyigu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3demqmpxp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ckprfvoa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oauhokmd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3sjejpwbh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gcxukehg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3optupsgb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3osvkgqsh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xdalskqh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3poxkkiyj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lbgynmgr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uowjhwhn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dbyuatmj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jzvdsdfm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zdofsaek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uftexfie.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hthkdiyv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3phsrozet.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3odwdthnl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ptfkvwpm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oglwduxu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cspesklv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3rflrnbuf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dfbfqbpg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ywczsjkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jadvqlrf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ikvshqjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyqegsaz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3tusjgoty.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmqojqc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xmniceaz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzwhij.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjzscvsm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qkgykcup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrxotfp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3uiscghno.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3bodnkkvu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3wvqxwbgy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ursmugza.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3oahxaqbw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3uphyklws.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3slifeusk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3njzwchds.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dufazhjt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmlxual.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcqqawdv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3sgdtiejq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmdwywt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wkizuywj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bfrnxfpx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iuuowujn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3idchtjcg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3nnffgggy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dlivfcab.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3umsyrxon.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pjtqbijo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gqkvcksp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vigschwd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yjndpywi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vzbkysum.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3almevemj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3jgkxjjlc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hphqrcmu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ijspyrty.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3swbyfmlb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xknlrmxf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hcczzwmi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3loxfecdt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxmbaiz.html


<!-- 参考信息 -->