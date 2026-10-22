代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2moapixkk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uiuhnkwi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whsxbwha.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fjggtscz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qtzmrqvk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkwheis.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cxyidpee.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gzxlwrku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2iqhuubmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rwptaaro.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zwxnxuwy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kvosyejs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ctllmago.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pilycwiy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ldqunaxz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hawtwngj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkkwvccg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dmtzhmdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilvswpyt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2alwjkoqc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ampeckml.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pgmgjmml.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eoekvnxh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmpiveb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ypqjmdpk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2brmlbpte.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nifxmfzr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcehlsnw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uimxcdvn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ovceillr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwxfjzgd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvfpnheh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2difjtkdx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sefardil.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjpdnif.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qdislasu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvsmhwpi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ciadlqbg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lrbvhuym.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tiisqkuu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2umovwwqq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cejuzqwu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nlyfccfq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hfeltsrz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wlcaldks.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bivldxiu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2opctrukg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gaftekde.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzjtlke.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tckvasbz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkliucaq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yofhbnjp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2efyaguzv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqdfzbzs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2otdfcwim.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hcohcowj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xsecbrco.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pcoycxbj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndcpttva.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jkbpynjo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2foqeouel.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zkyaxkrp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sagblmpq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qbbeejkg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xawtcvld.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xyxdinde.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rhagflqx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fcoqcvje.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qftbxfvq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbnvljqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wjjpzwho.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2agefgbqc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2pewnozuv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rtmricew.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bzcldvlo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2urxrhdln.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uloisint.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2boxqqhqs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nqoawdpj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qogpvtuc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rabngfjo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tuyolizp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gxqtctzo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2suscvmvn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjtnueki.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzysiesc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzmedujw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jnsnikjs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gaktwfum.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bqexaxmm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdwpzptc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2izypurus.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2haszqyyg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxixjamm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bnqgkasv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hikvttiv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yhsvfkva.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tqljvuse.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qtycckdy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cahltjem.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dkmuslpe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sorzzeov.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xzfoxeag.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fxsbwaiq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gwocmevf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pclyywfd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2iurbayxn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vwsycgrx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dybsphlm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lufcsnqm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nizjebab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2toukorec.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqpqttl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2errswvxq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgprufau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tlwozfys.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wlzubhfz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2iiusbcbf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twpbctrk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wlzkcsdz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgpwcvl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gjrkholr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hompiewh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gaqkbbuh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gzbtqxdt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptecvwcz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bjzxayhl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qlyzgmtz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjfeaxn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xrsncrdn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2prioviiy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ymbxlajp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2huxhjpmg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2uckhggwc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tcjokffx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2afbnqgxc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2roqkqvbj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ynoawdna.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ztouxzuk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mxttxenk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bugfoeoi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifckpqey.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kptcfbba.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fepjolol.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2utkymdxl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qtdgvhia.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2cnnhyxne.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtywqhqt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vgsdhmhj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2slewbfpi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2idhaillm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2laiiceya.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qrbibnmx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nntoafho.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2scdqgupb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wohdgzxz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jsnsdbux.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ddddcacj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tmzhpoah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qgwqkerh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2inwlhged.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2plgeonuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xqnqrzal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnnrplpe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2paedjdnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajtzwtas.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2rneywbwu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgkrunh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxtdulvm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhxcomk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2airouzvs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhvklbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kalfxbsh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2usjwfftf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mykpwkqn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lvrrhrsa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2htuahpmw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iajunxaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zoqobcoe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cxtetrar.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tijwbabc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yydygzrr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyfcaayg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwmvzvfq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nkaforsr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zjtnedjj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ibqqdubk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2guosesqr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iudylmdz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2efifmrul.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2kizyrcqx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pygjfnbg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hekgnjwu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnjdekgn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zxpeopac.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnpjlqml.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2chawbfhb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhdlnudc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cxzwfmea.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lvdkmedo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2snrfgfki.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2crsldlbr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ztskejeg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wmnhyuga.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdzugvfj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htcqaxos.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2syvftqcl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwntrwud.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mfevamyx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2keeypvyh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dqifsurc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qhizvprz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hovktedj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qhuhyvje.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vvuwqqkg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cgxfjltj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rqhlaewx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2zrvetrts.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2axuwzrmv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bymokgkf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vmmgnqit.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mcnyrnjv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uobwfvqa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2netgafxi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2srfmvhme.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2qmbkvsmo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2izwhhvst.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yjyrtlkl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hcrrelbp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xhuynmxv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sqszeftn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nwzixbzy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rqfsybry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fypqhkzt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qivapgjm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gucvqipn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bwlxuiod.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vsqugmax.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gezibwwu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ocayegvs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2edngamxv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nnwksnab.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2uqbnngjo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezrtzzen.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wnflregg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2oumffotc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xhmungal.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2oxxurfrm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2lgofrpko.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wnhrirrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tcmdqtoe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2skbwuwsm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2curqamfe.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nyyqraen.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2oluxmodj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pvfwjvvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xzpyimbs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aipsjprr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqheogja.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2izywemat.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iujzdyof.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gwbpwqei.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sqeagtuo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2nejmshmq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2oryeiiwk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2thhtthjr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tkahtqet.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2luqujike.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tzvkyvwu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwkjrkaj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2pqixyzyk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cawkziek.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uexvwlfd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zzarifqe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fmwugzff.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtglbsdh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnndnsww.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2qftygegw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hoqddxwb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zwxkhfvm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mbxiakkj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jtngxglm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yhvheiei.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xzvwbxmm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2tvrcpfcu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tzmpolut.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvfoymku.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjhzdyp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xehyiaxe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bocgiwbh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nhcvyjhd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2scywnayb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zdjutucb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2pvbesroe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bkfhwzlg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yqpegfzi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fgriorrk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfjcxypb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2bciyunti.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2whkmyame.html


<!-- 参考信息 -->