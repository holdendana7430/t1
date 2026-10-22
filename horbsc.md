代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akwwaunu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twlyfihv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dqwbbhns.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzzubrzz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmwgeugt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2juyinbhv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2klzksmts.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zgyarymt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2buiczyxs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zeeylesl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pubihbsu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2phlxqpiw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yulhyinu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifbyxqwg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hzjeurir.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pudstaeg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lzrdtozc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2azbcwrgi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2boevhxbl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gblxqupl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gfdfkknp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zbqvwthq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yfweyreg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gnshpnxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucyspims.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jmxolujx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eecgsuqa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vroikyms.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zfncyojl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiktamhf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwwldggm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsdrjnsp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2suogrrgb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2emakniii.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nmrtcsvi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eukahqdv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ewnlxutn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xvekcozk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkistooq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omkccaqb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ioqhcfbz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyptitgn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sckbiafp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwvplxoa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jvbruthy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nbwczsyr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2chimdeyu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gutdphbn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zrhgtwxl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2csyvstal.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nbywstlj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2keijrikf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zvgjginw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fohrdsrr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2sjulyfkm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gekofucm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2laqexlsj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymehghke.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2crevwgey.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rhpexjrj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qtgervip.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixccxmxa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2moyhkvak.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yirjtyge.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2grgscolv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdhlkfhb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2latiqrdp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iurnjpjq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oypgsatk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ygnygwox.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqeoibmk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmggqz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2haybcdqm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mjrxgtaw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2anlgzked.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfvpyx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sivbhpoe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmqyaehw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kbvgrnai.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sfqegfpa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hefoenkl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rrthoxez.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iwszdxhi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zcxpifvx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fnfywsum.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qoqwahnt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2puwwvybo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2srswzimi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ucrfbnxa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhwaupom.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tetbtfvp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dtasayvx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wshawknb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bsqzqnat.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cnfmpznj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zltbnqgb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kmifizjz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xadyqhih.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2joocakjg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvwruq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ixqulxkb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfqqbmlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2brnvfkuj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rekbnnrb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sfmdalpe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ytyqnkrh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxdhotgu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tjpjrwcw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tgtnbzdd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ggajpqpc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rvrkcrqn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kbhpxxzi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rbklrfpn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pnrewxjm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oujvaibh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ypiaixwd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mqekfzmc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2veodzkvi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mmnicgcb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2saqfkpkk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cjusurhz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2buxfxwlo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjiphfm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvhnqhp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tplzvppd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hdksufkk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxiirrbj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mkjbntpy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdgmrlby.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2urozeffx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qnhfzifi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlmzntfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qpiatgca.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uxssbwxv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wujorulz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ardtjyfd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pwimqtxs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wbjpidzp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axszfiyx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pihinhbn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ouaiqgpc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cfdopupl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yvdheyfz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yljocatr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bjhjshki.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jwjaygjn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2itttokrz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fyaydhyq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zaqovivs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fgtgmaot.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tbpucesr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lztabbfe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pmbyhico.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kcihbnqe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2seferake.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2omhnxayi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fzajhcfk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wekbjrxk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xavcuapi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2veqecgva.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zkoqfplu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zugmyiac.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2khslxihw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pevnnjsk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xpbbumok.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pbbvsiky.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqhetel.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dgsysrfe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tzqgwodr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bxhykxjo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uzjccahs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhvhzags.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2agtlikou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewslairk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2itrkxcxj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2maurmnai.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2igfmlvkt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzyaytbr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ilfggztl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2osklcudy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2waybrxih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xxisvuil.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2merxinaj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hsgljwpm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mcjhzkao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvnlgmwe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fxrapatg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2imbplxsi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wodxyihj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dcxpqvsm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hueibeqh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfxxoodd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kwsxidiu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ktrypzka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jcfsoftp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xbgarqwk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gfdxbewx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2forljxtn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ziiwqexj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wstfokcf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ratfnjmc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yoprvwcy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2crvrrwdp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2scxybhng.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2misjeknw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewgycasx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xztjkiot.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2aubclcds.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ezwamofv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zwupkguu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ppsriolf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2myjfhglj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxamhcbl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xdaehyum.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kspiksor.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oszzvecm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2infwlasa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mxqjpbsl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mphfivxi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bgcjbfbi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2frbnpeuv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mkqhaxyn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zriewelo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pckcmiec.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bbacobuc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2caknemlq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2inuweszt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2naxrpdpj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xzsafkpn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tgguwadj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2svxvzloc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkydefmd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rzipxvab.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ponspcdm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hyxnymju.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2sicmczfm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fsesgndt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2upreumvd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hdcbdsor.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dcyrvocu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2htomplgq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eepcesfr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2czskqmjo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qrmrizds.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2woaprtvc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dcqgnlfa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zhytwhyu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hmknuvuj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ukjxvqmw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lwvsvntt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hgxkhdgx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfahznwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wzxygszf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2lekauhzl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tafkicgq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fwefvnqn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2hiykveoo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hrnefoyi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lxgugojk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wtafvwqk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lczwtiwn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dsczzwmk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2edcidosm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpwgkqtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgzkssjf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2wsvyrcdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bihweucs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jdbvarbr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xuqbpsid.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpgpwaof.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gsjyxdpz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ferwjrnr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tkfauopb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rgkcblly.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kdiwwkyu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lanzbjwe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hqkdtpxz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cjwbghlt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hhkpounu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vsiyfwmc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2scouagsw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ixbttgts.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rljsrwgv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xlgyeyjl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qwkvpmoa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2anmqlmao.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2styexgcy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vmgdmacv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2yiodzkhx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zvxktzqh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jdkbztyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wgvfvnxs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pqmxddmb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2rtdbcyer.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2apixkqkm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2egnouefe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjkxyjyl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hpkeiqua.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hvefxyfg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2alfhysyn.html


<!-- 参考信息 -->