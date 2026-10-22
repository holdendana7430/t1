代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qpzabqzi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2byldgydu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kfaobnkd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jocecjnm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dkjrmvej.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oavvwpek.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpnrxqyh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gsofxybl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmukmxtp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzcgqhpv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2chkplglx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vanuqaac.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgepiaqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiulhhix.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fuarjqsr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzjtjlbj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gbvnoazv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylxtmxur.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bckcaget.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxzjxzf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bsazusgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksbewokd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pqhbfabv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zdbkrhve.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hkiictxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2izsujfkv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ugwmzjsm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2npnbbwgv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2igsciyxj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oolehczz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pzhtclgp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ncbxconx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcmexcdk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2atjeviyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swlphpyq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tiwnkskb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2owmovfky.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfdbwxta.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wwewhapo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdpnuuwo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjjvsuam.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ghhhlyos.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnifivba.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqnyhtuv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqpbyqxr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fsaupwaa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgcukldd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bkgoxrre.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2oxpseqoo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaqdjete.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vmnrmonr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ffqckmng.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yaweyayf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hdvuupwq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qvsaxukl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2swegznwj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2buwghmjz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2abarzoht.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nlipcfjo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ysfkbfti.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yhzjumop.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ohfljutw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ofymunqu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nphrtbcv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gthbgxza.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ddenkxvz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsqwxcwh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxgrifmb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yuqwoyib.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2geqgiyru.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mnaaqtcv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2syhgjnte.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2znlhfinz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuxviycw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxrgwr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfnabuvs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nzowsuip.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vfzjgxjo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pirivvam.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fpfkulpy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kzqbmzbu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kirtzjno.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flbbgfuy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2surzhqob.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjjfxblg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hahqbajj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dznatixr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbyxrczk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vctsjted.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dyfsrhmf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ghuiwhca.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ugdbttzy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nloekava.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oeydbnnn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rvdjciua.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2elevnexh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vkcztapc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mbzcoict.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eljokwbc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xuxemkbl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmilwjlz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rsixnhrg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2girqvwvx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lanbmolb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rbnlqnbh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlrmpgig.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ugaemcqo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mtyafmte.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2avwpmizs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zyeikbhq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fejlxdeb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ayiulacl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wctwzdvp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfpjjhjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2csqbmvpf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vdbkfspk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2znbijkre.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wdjdtpsh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jczevflb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2umsnfbps.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vngjeiud.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jmplfhhq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2chcopzxg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uosqedlp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ezrzcsow.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jegfldnm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hiqeagmu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nveijrvw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2deruphlt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pscqxdup.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thswpbjg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gcyorbdu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2skavwjle.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wvwlxldz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqpkrupu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2usugsrzb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rnitrsgo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zenhmhja.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dytynxgk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hselnklq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmxqphh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nteiewiv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2psrhdflp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdevcmlw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jxittvda.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2npnueqgs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qcvpagsc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wuxksjee.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxqmarhw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jxvpbifp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fbokusmq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jzpijagw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nfhqlcex.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xvawvone.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lqzssykq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jwnyzjtg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hskksmso.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeoiqiej.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ayoxjnpm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gpugekdv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qibdvpyv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gsnxslzs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryklwnjq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fydxegfz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tzsdocnj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzzhvch.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qusvkwxy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pfbdnjql.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mfuojyfx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2myfbnvdq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kauizsba.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wgrvkiph.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2urzrkbzy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2esvrypkv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zoyufrlw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2scspgaii.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ipqazjgs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2keaewmiy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jtgqphrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yepulbkn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qekbyfiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpmbombm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2oskuxdsz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dpqlyixe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2arpbramx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dkgrmnua.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvyxldhh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwpppodl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gbclraaj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xyzlfaog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyeuxin.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zfkphmec.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ulsmnmut.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxcvsij.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mnyejauc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrzrrlvc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkmdypai.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nfppqect.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dgoiycjy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikdztija.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kzktvbaq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ikunyywk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2msoornjo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fptymcyx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2marduegh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xyijsdkx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwtqbry.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2evwwkogy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vwoultef.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ajmerecb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2quwupqvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttscuvbr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lsmrpjrs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymkviujl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvxvyqgd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xrnfrgge.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzfmtrim.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzglcctk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jyoudifo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xrzztwev.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ymltqplz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2czjfbizf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2loicpdgg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikzqpxxd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tmrgnsmy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2couqhiom.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kzawnzdq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lrpzlcyx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fredtvtd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bzsnyghj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ztbfnojb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2obgwqmmx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2punfbegl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zadxkbfy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yiulbnax.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sldbnsze.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nkctqqkk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2iednvtjz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oobgaeyx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2taswbscj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dvpvmryx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2qwdbxzgl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2shzhkxpb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2axnkwkab.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2karhvpmm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2odxpidlk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2juigrsuu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rswldtae.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2fwcqrizx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cjahwmxb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jwukeegq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xnynugqn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wkxphljk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2cjooxqkl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2yacnnoht.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yeigbviv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zwnhgojy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iibyhnuh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjtufqcv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqlldcoq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zvhcorwr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2obvcxayl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dgdtywjt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2aduzjxkk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2byimhmqc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jhvguump.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hefkster.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2udinahnk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ryqxwnkv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mbeczthc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nhytxzqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2huysddem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twclozrk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ahkivlsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udeoqonf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ketehspx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxifomft.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uonygxsu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tfardksu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aidcdopd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ykbcdrwa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hzbrrmwu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2syjsezhl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cbdggifd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wvgszwxf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qfihdlqr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vcgvfzzc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hjtyllqr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ttatnikr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vcwizlon.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsyvmael.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnevgeh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbptznno.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vymrezqi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmjybmt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2craswexb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2orolliwq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wzjpoiqg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tixtdypb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mrarckhr.html


<!-- 参考信息 -->