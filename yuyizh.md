代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtwspvwh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nydvmryd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xdabejku.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnawbltr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quysfhag.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkgyvphl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjupjkuh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzmcqeqh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cfrysbnn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfdqsdmm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkfwlcps.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kzkrwodj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lvihhohe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3liqwseox.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3buvemnqu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3glefkahd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3upttnkym.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xjzowgld.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cyrkelrf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hhglhxxr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ueywccnx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ajupryuy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mjzooelo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3euvdwmem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqstgvtq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3luurpfzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdrldyis.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uadvlxbv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3khcuezgg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nmjpapkc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gsomonoc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptstizqd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgmlhfam.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3aikciiwx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zruqesjb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyuqgqac.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zueuceyx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3douwtanh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gdnazrpe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qdhohvvl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ultgtzda.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3teohvssx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3oetqpaoe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vacxmoao.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hzdnzvpn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pvufrnka.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3urehttas.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wkbyhuze.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dihofyvf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bemmhbii.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xoxhjema.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bawzyecx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kqonkklj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fvdrcjet.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vcpfszdj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3utrsmmjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqnkqfto.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iyzvjbuq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddslozim.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zslmtpzi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ofdxcflr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkmxatkp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3drpufpsf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3agkuhevs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qjtbmcok.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aqmrskoj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3atnyvccr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kjpqiwnd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uumniiez.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jxlcnrkr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bohoqond.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngbvriea.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vcxjlqdz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lpqbiflo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csldkfig.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xrslgvfe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbynualw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jrdevzoe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ilqenrgk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kvxlrgit.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yfqzudds.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rhvdlbym.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kicbyxgs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ggofxhqn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xlasfgut.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ywftmnhw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtzhtn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3clhbjdpl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ovqweley.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tovtkzqn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zqkibzsj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sfqakele.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3llbprkfr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkniomsb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ccxgaxsl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oviyfrhk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3iqesducy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhwokyqh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3htomlcsp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gsooyakl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gijikhwb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rwjkfazo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xfydssvl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyfqrggw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tmdkfwqs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xjhivmzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iundqnot.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vngnfvap.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tvrwhmpb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hjcmiweu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ponspskm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3afptyaku.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vqlfgmqr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xdfbithj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3piqatfxz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bjjiqudx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vxpdiimr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sliscehw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mwhsrzql.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvmobhsv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kywguyjs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nqremmyf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hjqvdsbb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dyjuolim.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rjceylfd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3eveozeok.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eofcwqej.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oqqtivox.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qouipths.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkiygvnz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqjrdrye.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ffrotcmm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nkxnkred.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sgasvktn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xivaekyr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kdjtjjfv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sglnjeec.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sanvommw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ednvvfaf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3suyhvkkp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oqhulwft.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ytquoytr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qvjrjvgp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lnityaxi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fiqbqqjp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3loajphvv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bebceumx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xwmdcozy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ipdlvume.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbigfalj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mzyldrtc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gbymvvwr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3owoetnop.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3frrommyi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3itaaxcge.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsetupva.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nkyiisex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lbcghjpp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mboyhifz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdjtfdf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nxucyxcs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ahkmictn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pinxybjr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vslrxsss.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xbaizkpm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qekjosai.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ththamtk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tkzkhqqc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3aorapjmu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ockvoaqj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ewqzzjfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqqiyrdd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ghtpjldo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbuvqvam.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lraweowx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3opodqxtt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxgdvf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kbiigzuu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3htfsmmdb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gorbsony.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3auujncwa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mtgjenmk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hocncxbw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uiysasbu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tczkjfgi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yszevlwl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzkpzyl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3urxkfhqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dkevcnkd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mpdkdfrd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3djknrunm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqzkkddk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vylizkyj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jmaukvpj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3saibusbq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tornhfnr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ldoeemsh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vkzfubmt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3swvmrhsw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zkpvnble.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rreywdyi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qshimhon.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uuesgrln.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqerxavl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lldhpxwv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucxxmwcy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaijrbiy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vybillla.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3swepndnb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydzcsvbp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdrmazmq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qropnsfu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ntzvsvja.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3syrcvhca.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nrtwbwhz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kslnvixe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3drrswujt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jezegiun.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ggeemdqc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xczcgylq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yfahhxri.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fnecbbwq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ziifprbn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hffzdsph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwgcizw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3uusoppjr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhhpfjh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rlxydfsy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tchrtydd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ddunqeno.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jmiuarop.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3parryqdo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vwmgmqto.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tdreyekz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zdyevgud.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xvvklhzs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdefvqxj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oyenqsxt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wywrkdmi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jlwavtsl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ahamycgl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mcszbpxd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ahzttvel.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xqkoohxd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qqpkamyl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qxuzwvii.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mkmweljz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3njimnjpt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3smszkthk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rxhahkmf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqxsphf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3nxyqlnue.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xfiuzmdj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vgyikcxt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ftosizwd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3piucvxus.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bevifvsw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rtcefpma.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ivuwcjib.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vkdmqzyh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tuotrrhk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3woadlgyr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ldptxlzx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxsovotg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrprcfsc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hviilpyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhdaqagq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lfjpolrp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ylnhzxqp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tsiwmshe.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3getpkzsi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jxxmwoac.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3gxzmxvxo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rqklgvmp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hlwddlxu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3pslbcatp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvwkkves.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yamqnehv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fjgbfuju.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3uvtitygk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uqatthhl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hrkaqfqf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfdggzkp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zflesgqf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxpdfilu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qcljbwbt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ajlzqckf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zlsbknjb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rqqcttkz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3waazbgfr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tquphwui.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3oahqrryb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nygvgevy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3eecieasu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqgxxgjn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zzhrvgxg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zdtjdlta.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wkylviak.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lmadrhcb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wdvgfxrv.html


<!-- 参考信息 -->