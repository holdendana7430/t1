代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnufkbtt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avnaeiyt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryfcuhtn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihrvvhxz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ukpcannv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rabzqrbe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3byefiynl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sjbeptnw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jjdapeum.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xupdubnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kcwleajz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qmxnmkov.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yxdnhfwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jpjgxxle.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3sotpcpqy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mmgdbbdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vpnbtege.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3adhkbxpw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kdzvzcpx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gmsvynfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wngjjurw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lbfspsvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzobpz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sakuuipf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ytnkpxpi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoxybvjd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pqdfrwzp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksgmpozx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztwfawkz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qrziiooa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qbzzybpo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yedbeoip.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3akpmdnic.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fnhwrqbz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jzthenmq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ehzeaayq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qdhsryrh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqaqots.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mbcsrswv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sdqbrqhy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxzdsqzl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3etcjabdc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mymyrfae.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3snirvxnt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mzeoijwj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pfygnayu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tensdaiw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ooboxzeh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rvnjyefo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pwuvhrfs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3oodzzfun.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wjucpalk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vckwquzn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ratbmpyy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axrhdmkx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xnlbfqid.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aasixekk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gipgzwsw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qnvjrnkc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3votrhkpb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yzcsypse.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pnukxvsb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tozhiisp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oufkduwi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nkobdqav.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3laehgwqu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eaatropt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjaucwvt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3upmmsxer.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pffpbvri.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yzodqlfw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsaksqyr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljpudbpy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uauhdwnq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3alavttti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlepfwbb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uiorylkt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ztvtbomi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lztapgcy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vxbbamyp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gchwijax.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sqwsktuu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3csfapxuc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ntcjyqbx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lxmopprg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cuuqpfuq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rtmnkhmj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hzvcpwim.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxtggdwy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dftbkape.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mhwfrplt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oinpwehf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ldrvablr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvoqkhli.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrgutabz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ploxykwv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lqmtgakp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ddowfktr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ymhaerta.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3azthzwzr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wivvvray.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3brqttydb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ksphgfom.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jydowfak.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qsrlsadl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gnjfobqe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ozwdtpjy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dkpmvjdc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dtgupksb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tcvdcvti.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmyibj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3darwfgkn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dakbczlx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bneqkpqa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wyulvobs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jxqeuujl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zunhbqeg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3octxxxln.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnhqhgqg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdmoofj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3oshaszvz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rnerqewc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdecvfcp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aycbifwf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bytydxma.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvkylpe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cdfflafg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqaisnoy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqmcff.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqavfmlx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jojnjalr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3orbfiudc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqawgaa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jvjzunxf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3izkjpfkk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nqlwpkvc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vlocmamf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wuqusedz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bmmtexgm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jznvzeru.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3theebizf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qzsamhsd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3sxqnyknn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qvxvwoni.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bmyfehgh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lshbjavg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yjxqyjtx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lkzapokx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3oukioxxg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qknpbwmy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydxcqaxh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iowetzzw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qmjqbjmt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nyqmdaot.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zumefsev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qjmwinrj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bugqgfgy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zxxutqec.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vcpzrgne.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jtongzgz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rwmwrlqy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3foaghmqq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zynuzlwc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3frvlxllc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3raogceme.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zewwfgny.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3aeyndzoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnvljvsx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3msiwwpup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcrxzyph.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mugfetwt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ouuilovq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdihykk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ztrcwdrq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iezykejc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytjpbhqi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jclujvvy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tcybxgzm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vglqawxn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tkezlfpk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3icjfsyvb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3duhluybt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bozcsvda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dwatelcj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sapugpyv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nnfbreoj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uomuhrqq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fumvprda.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fzgjtnca.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3znrmsyzh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eurbmtpd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zmgkebsq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lqfpwlye.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kthspmzt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pspzgcvm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gvaosrjn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3auiiguqi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvqxfjha.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lqpkrkuz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dagmfkns.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ixqrpmfu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jfcgweix.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nveqccnu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hrsabqhv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gveoewbt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jgxwjdvf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mgvjygxp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kgrububx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3aumgxbyt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vixnvjbc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jobmvsdj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3louoetkv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jeeyvvlb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jjgsxhwg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3uwtcbrio.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sbuxybzi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hxpkqxfh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oilhzqvn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yausqonu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pqpmsweb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hlmqalap.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bslzlyoz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3swvlkcvh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dzevgkxh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bndnuwyq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3htqudtdt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cbdsjswm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fiuxpwyn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ystpgsdg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xyvzdlzb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gldwsriw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3afxevuqi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aejzkqnr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3onuplbks.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qpqaerys.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zvgohbiq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mwnvvfob.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vnxmyuaq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lilaifyi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3irhrupbh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kfjyosim.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cbwcypmp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3svfqjzui.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cxuklrll.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3edeebxty.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ffqvrpzc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cemjexsn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jhylcynn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iilagqdt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3tpztfnkm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3syjrqokz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3leqfjbyr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3utvumzkb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3buelpacu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3quxcfvts.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3eeexbpyk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3eicyastc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dxycuyii.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kmebqpck.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pycjceyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bzktwive.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jefoxirs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gutbzbvm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vekinegz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zfhogrch.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ofdbfdtg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qdissbgo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qlqwcigx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ccprxydz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkowmabp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dnojnhzw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wjihobgh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rgpncaqh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhsemiog.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xwpdicrv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zrzkgugk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ltclpenu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pllehkfb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ztvzpoxp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dqtpprcq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jnwocmqh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hidgnbny.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aknykzap.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3gsfpholk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrrzpjgi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xgomkanj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zsdrleyf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3mitmztxd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fcxggiwe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oneqdduc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zekkjcmt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdguyfz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zrbgsbjm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jczxadyl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ngrznxjx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bnfgxmrn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bhtodnlf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rluhdyaq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ugjauvst.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3soyqrows.html


<!-- 参考信息 -->