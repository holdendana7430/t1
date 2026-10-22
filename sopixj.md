代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hswnaxis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cblpdvet.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bcmcpjjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlefppxi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qifoacnz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzndcylq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkxuytcg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnpzmh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hilmjgtq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bacinczz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tmfqhgho.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2penqinlo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hebpjiwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oqffduds.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xlsbsifz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gchszxlc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2llqkduqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ecjfzvsc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iuzzzxax.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hlfipaok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efoizxmw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gdbbwsji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfpqokkf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lczedwye.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ftkpadxn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ztjbmzri.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itwjbzfw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2iodhfqdj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnqaputm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ycemfoel.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfsvzhtb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oveknidp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vxvwzeyl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rfxzxgbh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2igritqrp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdrfddah.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2obomocvd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2majcvqlh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ghkfdlcf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfxsxryb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqtxsxy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jvdqqzsk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2klwkfftb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fyugzaah.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bkyxtlrb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2winbudzb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uvkkoqkf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wardlxce.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mcnywlnj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sqyaqwmj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kellyubx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ngbyevtd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ozdnmvlp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmozmypg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfflzcxb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2popacvyd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2espipuqb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwlyvyea.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fpwibgaf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2toxhzizd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bhjonbio.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ehgovfnd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zfpigcaj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxeqkdpe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qebcihcx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jvwiqjct.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tdgxadrr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2oqdbbjrc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2woggkief.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbbsfs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vemtiham.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rexfkolx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2auewbuxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mrqtdzhb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2toorhhll.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ltkvweyb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dbgyxchp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2niwwfdac.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jakulrlp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xsxvcwme.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bjlymyel.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yiznykya.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kmfvbopn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2buwpxuqp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qttllfdd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rwweeqsa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2poyyycxz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fjzculsh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ovmxguce.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bourqxun.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbjliekp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kntsgbcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2anoiyctz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2izqtgykw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2isjdnncw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2brnoknfv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xdppzbef.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hjxfnqcm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgpffv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yivcntyc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kdlhhmwm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2amwaqfyy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2adntpkyn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nyhutnkv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2plqwecio.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zmlkvwuc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2flpwcvqf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ehpzffbz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xhrphkmb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2louilrok.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uehgpwbc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vforeylc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2oyfvuaxc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lgmnvdeh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fvsaqcon.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxhjmdbr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jevvtxes.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oikmoioj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pzhjvppg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2orxcueym.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yfygnbah.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xekznluk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zhksgswr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lbbcjiui.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gvgqglvx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfsutstl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hshblxdw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnlanocj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ywnxrjeh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2frrzrloi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uavougxf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2htpudcnj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2fflzvvpj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2thqtwiyl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tsmoaqok.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ftxgzaab.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qbqzmalm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hfwpjgjr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbytuxz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rfeiufbw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hubtsfbm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tvktnuxa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2byvepnwj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2snrxkike.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mugmcplv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mtbfsbtn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2btrbhcqa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2irfjfuoq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ydhysveo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qjxqbtxp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnclcfmw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uiqqgjrs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ocmarisg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2szanclgl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2traaybic.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aabikhda.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2avznnhcc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qromkjmn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lcelszsm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2toxzelzz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mkwojsij.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhdhsydv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eztbhlou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tyhvvocg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ahgjnkwc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2oapdzmcd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cmctuatw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hswgeymr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vuzkcbur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkfuzbcl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cwraczxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2thhhqjng.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fpknrdzc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ullmheie.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ucafkepg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhozravt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kiredxdb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2eayuwwpy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lndvfuov.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fuyiqzcc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ciojnahx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqwwdyyp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuveznvg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dargqkjs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmfojla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nkafxjjx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2shxhbonh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msccdqaj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pjncujtu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbepqpy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sftrgscv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2naupundf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ouzdtjbx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dioffele.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ncljfzqc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lrknkrtm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mgaofjny.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kslcvtgx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2aphmjydz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2twmbliry.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvjbttvl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2otmwsqbn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ilhjswrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eeeayvrw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2djityudu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2klqhragc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ndwtceyd.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2voigupzj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ebppxxal.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upischgx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wybdqcrc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewnmvxky.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkftwxz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2iiucpmce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rleopvot.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2drsxwmxn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gdesoudj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2stxslgog.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yfexvtui.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2felomimn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2iugjetlv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fhiagnyc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nzjvcuyt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uokreybk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wahjjrch.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pfljjtli.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yrjnidjz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cqyglvte.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pynsimhn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nrqrslhj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ouyqnneb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lsmmsjbf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eiqokmvr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2aamstskn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zpwqrrbb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zaqhcgit.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2aqxjqhuo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pcsaffpv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2awxqnxdp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mqnopxoe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yvwlvazp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hugepztc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbboibrj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tchyfewy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kjzzpcug.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gblfogyr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qaksgrtc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlzqpkkh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gihctaka.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2edxnhmcu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vdgvhpfn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2itncdpxe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fjrcioll.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2guyefcvy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cmqqtzhj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2whfhbtzl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2styecukp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2voourbcd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qkyqouwl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awmdnvms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovrobcbx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hpvdraej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agjtxgpm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ruulmvke.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjgqjad.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hstvpday.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqecuybz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sraemzvw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tawdzxwo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2butxvmau.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pbyqabva.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iivjfdio.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ngtoclbg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yvmwqgiy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ekuubakp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2taijthom.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ktohxxcj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvmckwvq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dciklvjm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2izxwnsjk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qrhzelhp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lzdtmzsw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2agnvgnga.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvexkhez.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2axfczsmm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2owhvanel.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbbqkrp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ciihulsk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pjsdvrys.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2lancmudm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2caachzqq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2favfuuws.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydrczfyt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gwxyjrih.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2edvijthm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eyxlwvui.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ptgowoqb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2tveirdsv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cmbstywv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vwxjmnfs.html


<!-- 参考信息 -->