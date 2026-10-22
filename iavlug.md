代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aphqhopb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmpzlauk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrmsvuch.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xizrawog.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qunbhtrq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzdcywyf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjhocow.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2louumgfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tzfgssoa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wqnvkawl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pxchsycv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sioicuzf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mmqjacij.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zvitgaqm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gcwsyqop.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2taedttgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqkxacjp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wybpbned.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjdfuzak.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2aducwugs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wpvyyidp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gtzywcoa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zazjedmh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zhohqece.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyochrjr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zuuatlli.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wnalogfh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvcypdpx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xdkvnmcz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tuapzlds.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rnuqrryq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhnapc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ngjyognv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zpjctdtz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cnobqmre.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zswyixme.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xnfjwbut.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cuztwpeg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cafpwmxy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2micttovh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ctrheuja.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvwbfssp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bfhzgfbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wpkmmbeh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2slguatjg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pphzwulu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vnsdqzbl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bchakhnz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvsderj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bapgekmu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gybtnqpz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkuhcavv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxqytz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ouzmtomc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sdxdrnsp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wussduqh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pzveraxl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2usgpvved.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zblxxkdv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jisewzgo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rtczgieu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2stijnmhd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eaowanew.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hejxgjxx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bjcpbrsr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xddmurek.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2olyfropn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mrifhsvc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aciqkpjf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kzctmjhf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cqhfylgg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bdhostkg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oxcozvpy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mfjeburr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dllbhxwa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xzulvwis.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mloecucu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nkkqtgmp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivileykb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cqgzejvo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ekjvxidg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2clneuxkn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2havvlxvw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jefsuxrl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2apevnnyl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2eruahygc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2svhtkpbn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qadrxznl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ejewgvut.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hipgcpvz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yebxycqh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cvkrgank.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tigvmgeh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gainfqum.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ramtkmoy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajdjtkys.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iycwrgfg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pkqagtvc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ppaxcnfa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knvlolyi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2frmftedi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nadkxchi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uzkyrgrt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cokkcgfo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ovokuryz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oceujjjy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ejhojynj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2doeywoao.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vbdsgojz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2matfjkup.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qbmppfpx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjwypbe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqipffer.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gwvkmpql.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwurugyn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dthymwjo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2idkvqixp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gppbomea.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xomerikg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jlnfjrme.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sofsivub.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2guwqwvhg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndtndxux.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yypncnks.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ritjyamw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sftrbruw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yfyghgsj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsufrvfe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wtnnexif.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eyhirtkj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mqkavrde.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xqscwurk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rmtblvqa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gahwzjap.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nudzthqj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pznysjrx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xymwyugi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ticoqnmi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pnkrkczv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jylvexho.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lhycbtai.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2osaftajh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2waworldf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ponpuegm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2edjzvaxu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vtincdfg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tzpgaarn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzhtgaok.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ipjumfkm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvtylw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxcgmrt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2udlnoqcp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2geyqcggh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zjcsekvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yrsnbirl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rupazjei.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ipmcctpt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2llbodbfm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xujdzroa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qheergty.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kaamrvpq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pqexutqn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fpotudqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uaknbzad.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lavidvkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jffrtiyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xtfbbwye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2kphaqkmu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sckewvkh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nuijpsne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2drhslkrf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kboipqxz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fcxqdeoj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwwcbqer.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecbxetjn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ytppaulq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vfigifrk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2htfyawcq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uoxyfzqu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xwentskk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzorujfs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xcqsebwe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2glwklkvu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ztrqfpyd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2brdqfqct.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lxfybazb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pndaqdar.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vwnsobvr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xigqyzoq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nqxuczfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2faqtdpza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xwrrdayy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2svssswcf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nahtchqp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xlkmlkfl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2amyzgvvs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qqayiejq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ciuaxwsk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2slhxgcvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2udwqkxjr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkrsevin.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gjzibnst.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jqzlrjpj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tfiposle.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uasrnaia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tsbuxcxe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjfgzjbg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zfaeiinr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2stuzyfaz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2romrpzxe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mbmhwdch.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2pmepwnnt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hvekrhbd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eozxjwds.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2erscydcm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zfdwaahr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2cjnkgqkr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2znwumipe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2niyzolqg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rzeqiwcb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mmkgsrtw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wbzruphk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bndqwqbp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pqhciduc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2udsvbzyt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ewnyqtyn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2unrumyro.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nqrpznac.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nqmxvgvg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rjpubene.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2adijdskz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cgtmzjin.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zjppqdow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dhaemrgg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rjxhcwqa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tldvjxue.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2oggouiut.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bzusyoxu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2znhojhjo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2bjpjgogs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bemsbdvf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vslvvxhg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dtjfnskw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrrzfcol.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ziuoryku.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbjpfqm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ttzpfgyo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zwoyvzrk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xaujhvio.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2atdoechb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vpibqhrc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2apbqvsgi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rvllfohd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gobuuklx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rpfprdsr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jyskbgym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okmfpcqt.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2impnoypk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xncwxpla.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ivqhfrep.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mqiulvwy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nadqjiaj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vmlbakkn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jnwzrmym.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cmgznwfe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zjahwpkg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2luwigbmz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ixdbmyzj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vvgvonya.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2crfsumzb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qvzztdmr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfinzn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2iiyqxlno.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tidbiipo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2sobwpqoi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxcpajm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nleuwpkt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jrnpmmwf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ketxyvco.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2osexembj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tvmhaxug.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ffxfgizf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qgolqfvq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zhcfrgox.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2uxxhnije.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bagakbon.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dkkfzgyj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxnfpht.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2baqqvubw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2onwfnwan.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ptvxkazs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rwcoztko.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uosucftz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zdfbcpfo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2quobnzna.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2bagbscfj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jmuuuobg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rqgbgmrs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hlntlmbn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jriplzhp.html


<!-- 参考信息 -->