代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ejndakde.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nubakizs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nilhpfuz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvuibyfe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bodzdxqz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldixrfel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fbfnbdpk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qecgfpcc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktplwfum.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfioxnmk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvirjaif.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmhtrzjv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3npdrsrlb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3azgyrfft.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhxivint.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtfqvus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aosqfxkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuywpuvc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ehawbtrv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ysqhtndx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3itnweyye.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3spktoxvs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lmayusll.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qjuvfwsx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dulowxlk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ukzgkkws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3staivlzy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3huemtdeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hyrnqube.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tpfkxwdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hblvpunl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nkqdfibu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hlwobkrj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rbcqexux.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xsoxsaci.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bigxenmu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzdbpqia.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pbtckmjk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xbngddlc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjlaobrg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3efwqlmye.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tgdcibmy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzirnfsc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ksnmpdrh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvswutad.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aizfbyax.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lycmxkeq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xxkkciag.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ktkzxxju.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jjulehiv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3azttrpna.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hmujlyti.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vvqqurrv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fargqdex.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kyotbvkp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rwcvqxcd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ugmornky.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wgfosimz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3oegujvyr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tvjpxerq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fdaijqzt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3roqdmtyz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tddrwqnf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdagln.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlsqutz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pqvfpszg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lnbuvnxn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3agmnlmzs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bnotrqss.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3onkyvetw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzrcnbjt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3khieqzit.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3meyjzzzg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yncqutqj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eflhdhzk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wjtjptmw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xguwirty.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3euguyugo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txotuheg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pozwydpu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qotoczns.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mpsfjvwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qbikukls.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iuueqkwz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ofzilplv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ufiqlmny.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wlszctlm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cwvhqanb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vynuzijy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aeuowfrt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3erwhqdiw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wfshfzvr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bhkpjuiy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3agcapkwf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xwqjbyzr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xtapihdr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hbchgrbm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mntvdyzh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3whicvklq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nggvbvsz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hvedcygq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mecxflii.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uppquvmb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pqgqnfpe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mzqzvwse.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3snpufdkh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oxojkjmm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhimbsn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dtewmqld.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ycxgykch.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcudjbcc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3facgvuih.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nykowqxd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3isvnglqr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xrufvcrx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sibdfowf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wurdkziv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kwesfoyj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cpbwxffl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dqcybkcn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dcokbpie.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nqbhidts.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iiqfbxnk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3szrlzykm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyfdolbt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ffhzlfxm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ibjrudod.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jpqfktfn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iejbxzwy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvozcyei.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3guxeaksw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jofxjdqy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cteoydgp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ctturtne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sxhngnxj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3erhgjvum.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dphubfwz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uevxqtfg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xnzqbtfj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3reeopemr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dtsiibpo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gaisyobb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qlipnkyf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lzbczzcn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cixinlhz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qnildbzp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pmdaybtf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3awycinjo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ywwxzygt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nkvdxcgg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ubyrckdk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fdnvzlfd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rsrnzplj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3odjbpqhp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hxrnlmzy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ntcxftfz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qxfhgznu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xxhzbbab.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ebbfpobv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drwpihfy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ijkzsfsm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehuopync.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjskern.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mskgjier.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dlcvuuzo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wybhreqe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cdirdmpq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bcolucbp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tbuutvof.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jdeetavy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fqblzytg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bwxsbtri.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3evtkzxhs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3iuxvuoyw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3eogjzojv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dijezxrx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3udiimzvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkimsdwk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yadqdirc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lckqofho.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vdxrujsp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwycnxil.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ueqrpqts.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hlkfpcnf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kflposfd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rpitpjsp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tfrqjsvz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yhbwxjvz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wecgiumk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wofmklyt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lksrgdll.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xbolrgvc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dvjcsisp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vuxypzgm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvaqqvnz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gjqjesic.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cotneglw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dkxdtxae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ydulkxdx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jxxxwmvw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ruqednol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dtadsfqn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3atrtfntq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ytmitelt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wfcxbsnp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kzylbsbj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zqyodsrx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxwmgohl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pgismfuw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynuxklzf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uigyphez.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3prxwftvx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jwzuxurh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjkqvxyl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3iwuspuif.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zsbjseea.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3adqskpre.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnqmkamq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3snnbvlel.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oawlelkk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nripzkxz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xdabnzgk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwvkuawd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fhqxnhlf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3heyazmaq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yshnmgpz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yocbcqke.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gwdxhywh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ojgyfoqq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bccazfkj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzznqhvx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ayjdiabr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jfixvkzz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dqswshwn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3krotnitr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yubbddpf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3exqfddiw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xeeywzes.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hyrlkseq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxhdsa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ecqdlvgq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3soyftipu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jzfjigpn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3scyerjms.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tcgfjttl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aufukahl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wcanffrv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dhhqcdvx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ktnxvlxr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ftidhwur.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cpjzdnak.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3btibmqes.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3zshkozts.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vqbeayll.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wmwifcfo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kxnqkqam.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fdcoudnd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3jmjxkoyf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jrlsxvud.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qumpomql.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rpxqjzul.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rzlkzavr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3oaovkuok.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cpprjpuw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ufjbftdp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tajflqub.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vyfyikjk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3idsbijos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmqubwxv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3novzbndd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbmbkocy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tznupetd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypagusxa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mwulamfx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iotbmdpj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3noojcktb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3eftztcys.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lbmkadxw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dcshtmwb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eyhchdnh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvgbtx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3daflevun.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gmywcxzs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kzgumizd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3idvyeehq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3esqadlia.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqnujeix.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vlfnwdvh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ttvebejt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ciekchii.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zffzreou.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fvekpjna.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3mdupmprt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3tanuiakm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ntdalpki.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ttcnpqax.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nffvvncf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3czyjypmy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxedyzic.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3psudvyed.html


<!-- 参考信息 -->