代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2piyztesd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czzjruqe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tbrsuyiw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxbbouxu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pasqborp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnpuqbny.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wiyxuagu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pganylrg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kwbuhwak.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkwkzzi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpxczgqj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgnxrgi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uarabcha.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmhlrkxq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uxahmadc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bnjjxiir.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jwuocihi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2orbnqxja.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yxzppziw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mfyrbyit.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ciqdjaqj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vjgbzbdq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iafdgmkl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lhllzidh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vthjhkgu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nbncnphq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2diyhixnc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nyrrjdqu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hyjzowhp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lhcskazt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaxbuebw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rspbivui.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2icsjcoep.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qtjdzzvs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nprlrrbc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fvyqgfwl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnlzdvjw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zdvujxgw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ykviqqfe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qfubegly.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjfzxveu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fkuoslak.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jolgkqua.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rlutjepp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaakdtoo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ajbcxlfz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dczgcyhi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ldjdogxz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dxxtmngb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zniqcizm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rypgrndw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jbbtocin.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iqppgpqm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjjtqvwe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tyvocmlf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qvrdanbd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gclhfeim.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cootrtjt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krsholmz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhasvei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2otmpnexl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlsdsqlj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ryxsejmg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rxbgywnl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2irdjpyft.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziujebtj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zcszphyw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2plvcdfdx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcjnknaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bzotkxjz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qnvwcttu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbpdvwkc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ruqwautn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bcdqvwoa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxtxbfxa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vxzujpnn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2amansrxb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdtjlqvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hrmpvumo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nulvxbuj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pympanom.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nwdofiej.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dmpeymze.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mphuphtf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nupmxuep.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hdszdmwu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2humldoop.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rfflbsgb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bixuhgah.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zouqoppy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ksfjyfpd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mruihvny.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqrjmgay.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tjcompbb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mlskmnnv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oivjjgew.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2crdigvjq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ezlzjgpy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxgpyjsn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pzjtfnlw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vxeufyzs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zpygheow.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pluwfyau.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2otcsiuzs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jafdvelg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkvdajf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ithfzxhe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzuaqqi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mauzlngq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nwulktjh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fmvqnegk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hwhwdrip.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eogxlcbu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fclpykcx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qtnirgpm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qqozmjba.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qsuvansu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tcnajlvb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uwavcfox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgqwcvjr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jnywcfxs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rhxeewxh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lovjiwht.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qawepdgr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xgfoztah.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nskypdhr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cntusjmw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2guaeqdwp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdzzjba.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gopuxbik.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2deonbptg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wsyaqllf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jafuxqvl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lkiwqgom.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bsopmmdj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qtuwqqlb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ygsrezsh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2djbsqhht.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cioczdvb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2onhhxehk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tevjmvsq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2otiesuut.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2utstiihb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mvxxumgi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aarukbhz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vmnnhsxj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2djtvqlxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ydmnheml.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mkhqizqa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swbcszke.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vttumkik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ezpjihsw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ymkqovat.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jcwqbkzh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfhyszei.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twvutddt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hbnhsbuq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vxcgfajw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jhkaatoy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkdzqk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ypvetqvx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cleeitfp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yfpsples.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bnoqlcfg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fahcyzhk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hnchcrlo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sieyexhu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2liipqusk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lxgqldve.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hzjcjrgv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2keewowoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snrnfogp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qrinxlhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gerumkoi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dbcbfdxq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cquczjhm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cizwonzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xetpxbpy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2linejuoz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pwhoniic.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2obhhutjj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxvqmzui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2egmxbdcd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yfybefny.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2metubfnu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eqhvqcyc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjobjpvl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akzdcpmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tusldtxk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vcqfhatg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhhwvfko.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tjcchnhc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tjefvibl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pnluvyhv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qzpssohx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rksdvdgp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aedxdhof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dejeonch.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uohiredu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eidiriau.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mqbmfikl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hjpadsmr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2otsnhlrh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mlxbuqrj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnfqwucx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jznzlrft.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qakaumqq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2uvsgejhp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdfvyuot.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyfcqlnw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmojxjhi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nklfonyz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pertsgbv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xubtzwcu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kugoxqji.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2yilhzciy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qvzgxecx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xhzbknri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgfymzpa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rydgcpkl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ggxzzsjp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yyaklcui.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ipkzfkzt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2caiykdfj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kvgvxhze.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qgfsecnn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbmyzui.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yeolrwho.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rwuyrvkh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yolgbanx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrviigyj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2owfhxclv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkvzvvgl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bvaxlxsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2uzikrhmo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wmzgvfee.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ygfifrwv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2axdufooq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2iwvthzhl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tnttznyh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kozvmdkj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kmlqicze.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tosdigwo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2saalycul.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2eimwnznw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nihtgjwl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ifwkavzi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fcezhtqq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2owefhhtp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bauoukum.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jrwbbwin.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2znvstkwe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ruefxjlg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmadvrr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qtyhbzyr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2eewrqbfp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2oxzcuqjh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dnjnjwkx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fajkjohf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qbakozpw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bcqdkxxp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2reccmdos.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gsvrhrqy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rdcxtlwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vobnthcl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2atstvtxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2teqiawwm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xhxccpfg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgesvjts.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2krbxvncp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpgxqhs.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpopacam.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tvreprhd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrwfpni.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mlugupbu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmuuhkzd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pwupcpfs.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lvthzngd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zapeikku.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fzznjfxp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2yahnqmgq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gleeeswj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdjdorgk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2sklkbdxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpvxtfkj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2zdxevnxp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzcuqesw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mfyvoitb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2offkietl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tyfzitrq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eunnnooe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hjxffmtq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ltiycxrx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qtirtelu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mrzuzmmu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzwzckjn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hregqbgk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nbzjqseh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bvhehafu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dlehgtws.html


<!-- 参考信息 -->