代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pjwkztkg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmidcyhk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yvckfhso.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jacosoux.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nvqbwukl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2clqxrpuv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnplwvjt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgiorykt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prtkifhf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlsbncrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pbwmseti.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijsagkpp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckmjwqvr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lotmvbpc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyeicjck.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpnrsucf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmmuflmz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnyaudmk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gayhnrgx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2umlnnnbp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2txftxpqd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wckmcwuj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ipauhnvz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2djqbbzdl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ouhszntl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wqrkuhjk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iftetzwt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qwwbhdhd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hssvqseh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bhflcpas.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ndxprfgs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bvfapajq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktebqcwe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cfotxlrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vebieced.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qladwygv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lmfzsrdo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twtfzvrc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfbsiwsj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fjbjwvib.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yljvwrjs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fkmyolpu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjdofkjs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxivdfqh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2aqaiizix.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qqnhithv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mbrgdajb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyocjkk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saxdqrho.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ypjcmfrg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2biwkmxlz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkuqscdk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nvgohyjj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dzlceacf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cudlshkv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jwrshvhu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jdwylvdh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rzvbbzcv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2diyvconr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rpbhvjcy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2krhickom.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uwaherhm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jbybtqxk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fdgmjbee.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2emgccdrk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoggwbag.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkyezcjn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2utygjczv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cnffnnvc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzxtuhwa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ntybnogv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uwizunjs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zmlvprdw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phyuhtrd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ljcesxqj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqhcamcv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wnitehrk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rqlkvrpy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcmhcqym.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbccksde.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2etnhwvlh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xmxufexi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adixruim.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2axabbruk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gdqihiox.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hmixjtzb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rwhfaxhk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dltzwgod.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ffniktbq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2axvpsxnd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2innsogcc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhsssfve.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2swsjzyqm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xuiintcp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vfteceyk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsnnetkl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fdrewkkl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ozohyhzz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fwrzeevi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jfklhyql.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pprumsge.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dmpgxxby.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kruqtsea.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsxpltdt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yfaqnvbe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bbmvdfsc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gxoiiyxi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lgbpyqpd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nxvuzdwr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qmolrnhf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qjsuxaba.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dqnkdmns.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvorlsk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wlmyqfeg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyfntkwm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2abuiiiat.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rqoanqls.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zajvunka.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2flumvbna.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hjgbqsdx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hdwezwcs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fxfnkkqk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kwxvyebe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iofwbmpn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mwtckpro.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2thgdeywz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2neibrfzh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrbfhqc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2poiqfoef.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oftbkaby.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jysooarw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hyeypejr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mfxsjzyu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2purielzx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kairakwr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2twyjvisv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzhvvb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpphry.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxkdoqo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czarkock.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ydekcwup.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zlvuxwjm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2elzqwmdn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqidbjuz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jlsbjcuv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hwxoejiu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eafbxrcr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ojmlyupq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mmjpmknd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gatqqdfj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ghnxoeso.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dwpwwahc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2udiqgccx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ywebdpsz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tpittcgx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bkxkkjvf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ymmrutnw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulnxchhh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qxxxbktp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xdhdmskl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ttgaqwfr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2esdbzhqh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyzfvcgu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cxdvfclw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tgssxpzu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iaxrnigz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wpwgurby.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lzrwadbt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rbjmxgff.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2khjbsdfg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lrelrdls.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xuralyok.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ractdbfo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjsurbys.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vsuqfwti.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2eiobmvir.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bqvrdbcr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2shooilub.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kxjrcdtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ueboimhp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hjacmcar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjbnpzpi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pnmbqbsh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wceegnaj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wcuuobng.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ljrrkiml.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzsolciu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jyhjyphz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dsfhsroc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rvncvdnc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2cwognnpl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yadoyler.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hkgdwest.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyebwexk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmdjlgf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oqwczffh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uwvbphmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2taehjpby.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ecznpizk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjleddd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2trstcoer.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jsfjvllu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uapggabf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uilgtsxz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bgfwnbkq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yxzoxtue.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2yovbqflz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lzqwuyiy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2megzzmzu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hkthmmsf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qgttmyys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zhwrojmv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rzasuevd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2srtwxkoz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aonmwssb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2unxmbbpe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdtqigyb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqsmafya.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qimvyejp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2twuwtdss.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kiplbawt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dktvubbz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwfiadvr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jomfavle.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fkdrpocj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zpvznwrb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kqyegjjj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2phsfjmoy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2peymvjea.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jvzckxer.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pzqnljav.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2digdgucj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzkprix.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mraxwseo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lxetdxoe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2isafoqqw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2axpceuhx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qaoffhzq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bdhlykvg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ffolaijd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bysuqzyg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2wmvflsue.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lyzedkus.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dcjkbcgo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zfjnxbku.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xhwvgfjl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lvnxvtri.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ofnajqgg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ikvrbksi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2okswswpg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ygjeuktj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2emyloeum.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hboegomq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jsdgfodk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cjohmwtn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2puqtzfxi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2sqjvrktx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rdjynuyi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2toxogrlf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkklwadx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2jqrrkbui.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqklan.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uzpewhin.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ptvakhbe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2bwlixiax.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2glnbnawl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bdfhclmx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2socbornl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zrazoicz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nlzpstjx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jtcqkljx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjyoaaxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjmygavg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2muayizrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2albcfyan.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pvqyleie.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bidzsybp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jeizzdfs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2spohtxjp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nodbewxl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cmsonbza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2epwihoqh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vllulaad.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pylgojuo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vyjbfywz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rrvqlrvp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fxbhwidc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2aqgajvdd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cqazntfc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jbbnvkfu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdiowkbq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qkdvzzmq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ybungabb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zugtlcbf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mzhemxcv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ycaemueq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ovfuwsbq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2pxswhwqa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hocseuwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2aphiromp.html


<!-- 参考信息 -->