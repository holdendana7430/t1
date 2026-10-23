代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fuffhtmd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rysvhbew.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3divomzgl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uakjnpek.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfuxefqd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luqibjwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3luksdimu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekgzucsp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjnlncly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsxgiipm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yshnqvov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmzulcfh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3meiuigzc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhljfddu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouzytsiv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqulmpzo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tiivwras.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3opkvcyms.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ggvpbzdu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3njalggtl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wbytufcu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3befiixif.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hncmapwq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3koagsbdz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3stniajih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ctoyeuxn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ansazswh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3glbqofrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egxnfxwv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gahcavtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhhlrffk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bjsyggda.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3joezzgji.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txgidyvz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghnwapqw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qoedkxbq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3auttwwcy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3opvxrrei.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvkuzayx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rnrsuthv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eptqxxkc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lifagomc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgcybjli.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hahnkepf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msodjcak.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jccynrcz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ltowdkll.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bvtiifdy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dvlyaccs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hcwlqrnu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ysnvlgat.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cdnftbhf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nwdfkqcv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iksnyfdj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3glwlevhv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ceovgahx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hdwibzvk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ymhxdnrf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tdmkwmln.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nsxsjxia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkvhwcsk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yhfpsvna.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3psetedib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vsxntwve.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ezwwnopl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gywygmmt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cjpdaoyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tuyhubfz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ptagdekl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pvjdcoic.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzzzkwoo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjakhhry.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyzuwtcc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3myvilplp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3udmmlekl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3czxyzvgj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3htxbaqde.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kqsdedki.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvppgzqw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgbuldkx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xncqwbnu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dhwqkicy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3emiqtkzs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rjvtduzk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gtlwoyhk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lefqmqsk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3drkwxlvk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwnqwjhz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hvbihxio.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rjxnhtnl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3szjeusca.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lcjnikjd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bynzvtcw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xdqglgny.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zvqbjtif.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xatevnyk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcjfixia.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlybenhp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3azznteyk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzwvvihj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pkufnbxb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxqejfeo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zvdqarqz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qrsodkts.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ropqzaop.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ogtvoqjn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uqkhlwvw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3odycmkdo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3idipiaff.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ooxiwlxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mdvlsltl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fthrrznw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jxyjmhmg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bhtkbkye.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zlubejub.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xiltbvkf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xefwkqmf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3blmknilb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qwnamgvn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3adkcuhcu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zaicitre.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ghbhnqbn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pdfcyvav.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yhkoqifh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ipbyrqvi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3luiyhlfv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guyivlvi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gfmumsse.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mhmseysp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnkgsbs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mbllemsg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gczfmtkl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rdrkzbag.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ptwmqvfv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mfghppms.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgekkmzq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bucfvxbg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hkewcjuu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3appwmiqj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lodmiwcr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3moeknvvn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxxgizah.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wcmfqtxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qtplygcb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dvmxiaat.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ywtcayza.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jpoflwqs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jltssbce.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ieyigwcr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rvxouifs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rbtytmxs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jmabbnfg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3brlsoxlb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lluhbttx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nufkgwhg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yrrvmyes.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jpdecaxs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nytafhzz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrebusld.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3owkkadbx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uozqzmov.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bronscwi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bgntbcpi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvydtuq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3htxdxjbu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kucziiaq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bsggzkgb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3slhpcakb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3npaimqja.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xkeitftx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmlzxecs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lskpeipj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fykggyuw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ktiepzyz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oeycesko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adjyqrnm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cojvcpez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vshslzgm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dwjzjpxh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kicobgat.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nsltpauz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzjunbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojypakoh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehmizvde.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mkscwlmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nagjspgp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnbksdtu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ftbdwjla.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3diaugwnd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyzgfoln.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxhqmuh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3avexcikp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3djzlsozt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jyjgulul.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujcxfnya.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkujrfd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3devcwokt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdcvzr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvlxwelc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdlxqrvn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hzepcjfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3stjtvuge.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jzzugvby.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3irmtvolu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ucxaprde.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3znnslvzy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zchzdvwu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3glttbkif.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfakchlp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncyndfgl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vdssutxo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3slomfdoh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dytkhfik.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ijntxxhl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sudwylor.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dqeynffg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3chrcomzt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3byxfndbz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azmpjbze.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3blbsebik.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zqpnmstb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tdgxzrvm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlwbcwoi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3njkjjtlr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3quasjckg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hbuyonux.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vsueznmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zybqsjnh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbnzhpy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lovfoqvw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qnyoyuvh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3piwslviq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wuisudef.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lfxaathj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpmxleca.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gnfeaenj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xnwsqlhy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lyxthniz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ancyrjua.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ylmgysdg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jegejxgt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yroqwxcc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3dhbckwsl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dehzamiz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wnjswzav.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bisibvok.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jeswsnzc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ekvjxyii.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ybnppcdh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3beqihvkw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3seytvjnv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yaeughvf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zlflkxgh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hdokawfl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3topxvrqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pittjdbe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cbmeukvw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3iynendpk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rcncjxnu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ysombqoh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qkjfifbw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3gurdlaqh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wtawxbuv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3urwfrrhg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ergjcrvz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bjfaswui.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fqamnxol.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ngpdakxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dadxovqj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fajrhkun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwzobpcq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vdoubvow.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3doyywzfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbsjlbzz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kreywcke.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3htnsgudn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3tbqlutjv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuwmbrtb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfheaqos.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wykxcaxs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mykgbiji.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3abdglzfo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yfzslrst.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bqtsymkb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3wafcgkoy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nrhjsote.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgorpnqw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jsqzoatg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3thhqtokh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ppdthaiy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsgsddkd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgkdbl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wrpthkjn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jedrziix.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mtvlnfme.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3bstttdiq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tiuajmzz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hfdeedyz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3oiqytwru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfqlaer.html


<!-- 参考信息 -->