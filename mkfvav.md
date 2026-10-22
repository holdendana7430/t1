代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2corvryri.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcfanfbp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dvydmfvh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mboxgstu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgqkujsl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjvvmaul.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhduzopu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgrlvcqz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxacyfat.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkbtzrtl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzldfbjt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bcjoqnek.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xgzvwkwr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aiuaabeq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlkwpge.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2eueuawiw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dmuvkgxt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vhgourck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tvqbyvrv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jdgrnsct.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bjbbgdck.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zjjfxrjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tbhzhdzv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2giucsvgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxukqzuk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksbyujzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnxpacnd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2runiaevx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xhqunxaj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwzcuhax.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xfzeswai.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ecequnxb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2nyfuuuqi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cvekgydz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcqvontz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rdzpfllr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ccfxaftu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xoirtvgz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2khmvdbiu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcejehu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfllmctx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtcwbenl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dkckrbin.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2esvtvlam.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2urvuiera.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lugbuwxj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bzbvtqaq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kqwjedgy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sdzqqjbb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nozvicbh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2djvzeayw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xjfeamcb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2abihmrtr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sutzteal.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jssrzkwq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yphoqsal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2trvxdlvr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moykdtzb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zsocgwvq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nfynqcmm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2txsiiank.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmskdlhn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2csfwxawf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ozuupsvr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2emzxwqdv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwzftpls.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mnowcmyf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkpprpfl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ipmzaffu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ycfrofcd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zteafooy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2augriukp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pfcodhmx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2adpdbyad.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjvrhue.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dqfwozwy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkvyyhb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imqhwtlb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2blzunxhw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ukcecppi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2etnkntse.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqltepdy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ogsipeel.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ohgebtbk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sayuobnz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fdzzzrck.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ptszphvn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aqftzoin.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kkkaunqg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hodzqydz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2izgaqwno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cdwykxkv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gwvhvlti.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oseeuovz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lluxawhn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlqsspmr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cflzwgym.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmbgfywo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttphscji.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ayyxdyzn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lecjunlc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2csiquxcb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2iwvuccfv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2euzrfikx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ouhbloaw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lukmsenl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uutixljk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibqnzsap.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2becaxaln.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bfcfpzjf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jpfniivq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lbaymvno.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wasmintr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ystffopy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tcxliwwh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eztcsllt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2cygsuisc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kndumjug.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jbsseyyn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pdtnuwnz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qlsqnyin.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uklrbidt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2olxycglf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2irewkyqx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fncftpmg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2srjdaxea.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2amolffuq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rbyscdcc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbqxdmnu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fxbgnkxa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oncyqztp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihjzabwh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2npibhiud.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2agkzjtez.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bvmcqejm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zubrklvx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ydroburf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nlzvzwfm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdrqyacy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oxbwmsph.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pfpkueqe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bgajwuya.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcdkluk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2frcrwowc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oqwycawf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dmbbgmxg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cgkghese.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mefsqfaq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uhzjzftm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcayof.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqbhzud.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lhwajbva.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2glkdziui.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gdzaqpsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fmsehsyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jiovurak.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcxozc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lshgsaag.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kfywxmtn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jqrglcoo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cjnxyldi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjmnfus.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2topexprw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rntfgcor.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qhvccefo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ntvhtruq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2karhfebf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vygythkm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2clxzaqhs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2aiehzrkn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fsfcefnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbzrwcir.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xqbsjbix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywkvsask.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qgbzwmzu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2shjhgcef.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ddsttijl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcpnogtq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2saraeipc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ersylgre.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2caunebax.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ktbzpwli.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ojmduzpy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pwdfeofy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2egysbehc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jcnaysfu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2auvhofce.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysspzwkc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjkisjop.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yvujpwca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2purykrev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbwijjvk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2anmnauda.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tdrbidau.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whouixpl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kxjnmlao.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hcdxvhof.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rivnbbza.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfwrtjr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wxmnjigc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tvymhsus.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tbcdqajd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jzpjjiez.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tzddhjjr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vudotizd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2swzzwrtx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vnajpaal.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ntrsjfpa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2aqopctvt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqheixip.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fxnitdpk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2umphpbjd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdxrcfry.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zqgzaomp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkujdq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdrcnbxl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nioglcvg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oomqioxj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dukvvhdh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2svybdosn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ohxtyytf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iphwwvii.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bkpnpdow.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kusafzrr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tkxzsaim.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ktlszxgc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2emxfzpiq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iubvlxlz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xurcamaz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gbrmulov.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2myfdfqez.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fhyeurse.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwzamjvc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ouzyeouq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mdmntdzl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ybokgmhd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nkpoctik.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ywukxysh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bsgmobqq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ndapusnh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cgbnduwt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2umdshmtx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2dkhvfwbk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yapniksz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hvipgpni.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hmkwduou.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dffxirsc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2njpfljvl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rvdywxvg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ubktrrbt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gecfdgar.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cmxossej.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xibbetnf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qdumcpil.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lsmgpdyl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qdqxqpfn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dwvqfnzw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2unlyctwl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rgaztfpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ufjorqrs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hsszwton.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dxupqegb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dntlghlh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2suuyfzra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ongglxsd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fazkcgpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txmhyigr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ivmoknrg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2sehfzewf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmyloztj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mxmiedgp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2urpqkdrz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vhzcmged.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zhqdtwmy.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2doetvoqc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kvhiorym.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nmmawhpt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2amtqtrrp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2chzstell.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jcwrpkpw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrhbyrd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qhepuijp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2eiwcvlph.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2diceyofb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ochooyoh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ewrjaqoo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2cvqrkdpl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2osmmefew.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2khwngtsj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2aowuomma.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2djrhetkm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rpvtierj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hnaujjhi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2coicbufu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tfihlpiq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2grzutneb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yribgelj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fwmtjaat.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nykzzozq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ojlzcuve.html


<!-- 参考信息 -->