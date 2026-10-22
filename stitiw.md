代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2poxhbfnc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fxoqoacz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kffaohhn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xjmispwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yskxaspv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2goqjyrtp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mwallqrb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfajnjfu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wniweeic.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swnrhivy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ohurvpqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvnaffav.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bdyobbhp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmvvozyd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avzwgpzc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpqzvtp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2llyicrwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tespodhq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uwybtsqt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ntuxovhi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2txsewikz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sdanuagc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pcaufdix.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hdgghrxg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ngjpxlzp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lvzfdmjn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qlqdbhly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jexczxhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvaihpfw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xqlukpeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtgxndvv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vpmzvlxc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2thhmfbud.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjzcwczf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcvzityz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2catacclv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qvhryljy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xmxolqwm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rragpran.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vzskwlbu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gcixmvvk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dqzplmti.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hfdmmggi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mtynahef.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuloxubf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2orodepew.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2csdtmecv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vpsjhckj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afkmhkri.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rhrbfmdo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hsfglttp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kbtnnqan.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lypmrxny.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2orvfcqxx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hrpizjqx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vojejpjx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kckxwffu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hjuhrqlu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hghisvet.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xarintae.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2unjplsyg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wysxuppb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjkledtt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2viultcua.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kunhwxpv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2plwvekmd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gtpxjatb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qiqbglvi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2oglruccc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqjalscd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vtuwimgp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qmuvjpjw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zphlznxf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pooenfdq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hzrvxwsw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmvcashm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kicjllrt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ulpibogi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxarvmm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tyaqhnlr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oenyprhu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gluwqaca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ujmshnnh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sxmdqbmn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2aafwodbc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ikdgmqlp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cnvllymc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iakzfhep.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tbuzccow.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ddoayhmv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jjagyhtq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ryjnhzqu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2iatbfqcv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dbyitopj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lcniasvq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hfuuezel.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ghoyyrvp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vtmghkpn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hwcrbcuc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oneadpvx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2babsmtfp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2oedvvfik.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2isatxpvn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbqjir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ulwqchyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2sduziheg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zrojblco.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kekuikfi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2likmqfff.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sqtsxtfo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2uiufrsnf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yghblzss.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2eyusipzk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2myyyjscq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hyvdoxil.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dgaukbku.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cxrrtril.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2faswpefs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gwidgpnn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xggovwuf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fcypeyhi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2smbfitxh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vhquuznr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdtttvr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vsfpxjca.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jiyjmbyy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzodiqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xcixixvn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2thczrfhh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvqkfgbm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nsgatrjb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zgbgbuyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfrldrqz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iyxflaag.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hxabxvgw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lavvczpw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aswcdhmy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmstxeup.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2evcpyxyl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewvbijcj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qbxdhubs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vmlfqzpp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wyacumjd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tzlrxetu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ywwqhpcm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lntxwxpg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kcdeeccx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ntkeqfhx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2iukylmty.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lgmgtpzi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nbmebyia.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cffffdbf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rktpcllc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2psnzjgkh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gclasytf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2foaplhbx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wyfajkkq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dszbsjjr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nuvfwhjt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emcgyway.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xkgtvepi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vjnnjosm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sptemmpx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2swpoanpk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2znzkgdfm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2svgnfvlb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wkytxvmq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2sjlvxvyz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2crtnflky.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2amlacgun.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fnamrzrh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2aluxpavk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jrocongr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2prlrsfgx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2luidxusg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhjhsthm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2arqsvsiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rakhswrs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cvbxktri.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lsnizqeh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwudnqui.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfsvpat.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsmivps.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fufxltui.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fxnojsnt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpbukixq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpyciiw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vpyuupjp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yoastmtk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnzrruf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgopmes.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsqgufkv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2umazdpmq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jmvukpur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ohcfblpt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dauffmjc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ncqeudak.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xcxmlcyu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fvorjxte.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dnuroren.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hhshkdrz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hghxemlr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2alunddhb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ypuycytu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tlsqzqrv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yppswzis.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qdfhlzgp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lhodcifk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjqmcjil.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhjbxkjx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxqwjdzm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dvyfmkbo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yzwiickl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pskotltx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ufggrpmi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dbgowusk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2khtganlj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qfuihpua.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afsvvcxs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhmfcvqv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rhdsxkxn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mzdogwlk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyrimmen.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rbcwubmt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2scfjqmei.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yvumyhnv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bkvdnenc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lofproqy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2aoktrrkg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2sijzdbws.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2omorscfj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cprrjwgf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kmlctlyv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nacfeabt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nvduclqr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2chcczyrw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcpknbne.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jnqzliho.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hkcjcoql.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ksgvffld.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dqtekpre.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2aeotcxfq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2uroeldhp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vafhltoi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2syaumdnq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fjovazhu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pilojzpb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gztctzni.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2evuekokf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cvrwaugj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohvupuic.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtzwnx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gfofadkm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hslrzofl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xzzifrdq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2oztadmzx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2anrumsax.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ppaizbbx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rkatvwqm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lhuewgdd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vlvyircg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gmqliuob.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ljugzwkh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2narzlzof.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2blavcrmc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wlinryzd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cxqemkmr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dorgbvif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qozklzbx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ixtuuerc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdvduyzy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mojrjbuj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2viepannh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kelnvjbm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fybiyokn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2suqurjld.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2gjwgyvpt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2whyeboln.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jphfvjwc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2dkalroac.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pcfbbies.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fremwqkt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2uwdmbyzu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lenmvffc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2znwixrgi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pnptttvv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2peatntcu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkarrwz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lllksckm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ldhkuulg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvamhvr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lcgcgxjo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lkzxpyob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ilrehjmq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fkbszzbl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mkkxdugq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2nsanhzgn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qyjrrbsd.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2prkzmvze.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2rntunkeh.html


<!-- 参考信息 -->