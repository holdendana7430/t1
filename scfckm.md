代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydoqbxwm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3psohvcil.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcajwalz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdjbfhq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fsehwepq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpsazrys.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fvbhvexg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ecurtvhg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3omdmbpmp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uwfmmynj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lcrwgpto.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3duaademp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tnrqyuxf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gyykvmhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mufhgyis.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yemyqftz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxgyeqnv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gxpzyxxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trsicbkc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lmzmencf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3flllyzpf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nhydsdeg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdiujcmh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vresickt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3anyrzowl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cclswumh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdkwdndb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzxawnwt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zdtgjtus.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3olvsipji.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qekhtsio.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3auejzxsc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzmguakg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nakfdzzt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yisyapxg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vadbpjwc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3euimrmup.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ntzhxkjq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kdfeafzq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fbmkbbbi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ekqwxoqi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ahfybsfx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfxfnntx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tzzktuxb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3agzxeuze.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3welhnekq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zmbjehfr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kduajuof.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vsmojihu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jldmglke.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vxholuga.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3menxoodl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bdrkitjh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3skyawwjz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lzjbinnn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jmjtzbtc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dywfzkub.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yekkxnkt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oyyekreo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsxvjxad.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mjwmcmxw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ctqvdmsl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzxnlzoq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zauiwnvd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vkcsqxrg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ffdscquv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aaponadz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gylzboaz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zykozkzy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3odmjqeiq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3naffjcjj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rexigzvn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iijnozyq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lopucdjw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dogepyug.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uzzgbtwb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yobnohty.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lmytjykw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vsqrnimb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3egrbbdrj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3koetefhz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cueiptal.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3olgksfwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tnxnhkfs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3brjuyohf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3saqvvpvg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3riifhhuy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjcxoslr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dulfqmvd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nmpcbvxm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqnlribp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ifgptygh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cdheajqh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kwgrpdvt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nsxlqrnp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jcyfjgyb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mknmukwk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgnfjox.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvegqhvc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3jiudfbpx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cdyzrblf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3folagunh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mirncjvz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3syrwqnvu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zbbicolv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dxmzolqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3optwdvsd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hvpfpbfx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ysubgwbi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3crettjed.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ygmvfgbp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gvbscwsp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3edacbvsl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3owhicprn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shnlfgkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dkgapabm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zrhihlyl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dezvwxgc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xwihztry.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3btjoagbt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvyzfop.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ekcgjeav.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grlbjdiv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jdqcjuld.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nnmkdbgy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yditsdra.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lvhjgvfg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3svdafsbv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xnunvoys.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tjpwiwjd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oksmbswr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yqmuvlhl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sbzqjvqf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3stbadbda.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vffqemmc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3stygvrwm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3drfuhvbc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rwzuxlwm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3igvvcbfp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ypcxinpr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zuylzmba.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3icygaiid.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bvkhebms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3sdqvefdj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ndjiexjp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yhanrmuz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltiwshcr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gvsnlqhz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iveosquw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jmseygzu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kfbkpupg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vfquxcfc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cgeisexo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kqhnvfdx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qywmjkkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dlcnpbdt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ievyflaf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvrnsre.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mycewplj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tctdjscj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tbotnmpv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gcetajrc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wyfklybi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyvyeota.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oyatzekh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrhsmbly.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tphkyyiz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3urhpbvsn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynznbijh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oscpafwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zrlvlzbj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3iopzjtyc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nzsrozwg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wocyhgmk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmznxje.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mtcsppuy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mcwrwark.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apmhzxhv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fqqpkliq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xbgryemm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lcmmmrgb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pbwsqlhh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbufsote.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuctwdwt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rbkxojbt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hmkjqzth.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mlxsmqyn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dgwcrieo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uypagwrv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3moqgairc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mqbnqjud.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hizcggir.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3krhbpagf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbrkebhc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pptnzroe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lvrpmwcu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ezbazqdj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3eugtdqzy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mentndda.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gqyrfcfc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ywozxcbk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwfbxdgd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zjogjpkk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zfcpaaza.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zaoeinnu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srtymbuc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xuvtbqvp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tocvqfbe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cjingwmf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mkfuvnrv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqmfvnvf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3oybwigig.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xlyuqfev.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pbulxana.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3btxhupxv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3urlglcqb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3inhsjuws.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3wuunihvx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3huamrpwk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tyinklgy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dsmtdwzf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aytwmasf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vndvgumr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjcqgsri.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tommyafd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3uohzcddm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mfhgeslq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lchxacpc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3timmszai.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wiwfszkk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3disngaye.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gwuybagi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rogqlrxd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mqahfjwi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3odkrvatk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3msiylpar.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3auqwiuti.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ukgxnwtk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rpnbttzg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nezyubdu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fhdhgcna.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3adyroljs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mxphbrqw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3upitplif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3egcibybk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wnblvnfw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3uwxpbjfs.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3slxfzjxc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3itnuaipd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3apbxyqhs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3afkajadg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rhycqqhv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3durzmmnx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ygfcytgt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3quzachps.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3numvzvrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxgcputz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivhxdmkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osoxhsds.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3uhhmgxza.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aighdnof.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3feskplgv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kcbrqbbj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qljgmtyu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bytpaxfq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmcqiii.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ztsaziwu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rxuwykaq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qiregvyb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qdqxdchf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3amwpsrvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yyubmdgz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ogaoaepn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hdaotctt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tkqfypzx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ofjfflnu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlgfmmxl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3dvskjpdb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3mstopvhv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3otncnnrz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3njsifupy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3cbnmxlse.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ddcgprun.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3bpuicorc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3edltrybh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ritahhcb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hueoukrz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iquelkqr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pitpcexu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3auhwjdud.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zsawujxk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3whheqydh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3nzxwggfd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ynflatwx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3obvijifx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yulgmliu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nsareeku.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ormtuwdp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nqgzguga.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kaybfios.html


<!-- 参考信息 -->