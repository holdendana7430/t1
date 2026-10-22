代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gokisght.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azijiyze.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2omibypuf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flowfcij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdsbpqjn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbpopdns.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebfgmyqq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2naizcpdo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqyqncax.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zenpbolr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zadpitcd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkibbkww.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kjosqlbw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahixlznj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hwxvhpjc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sghdcckm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bdnqawwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gejczsyg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2tjaywbcl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kuntwmal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bfdyjnae.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jzwqbidp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2brhamiga.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mgjpmbxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msnrhjti.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iwtaumpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcqzbwet.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jzfxerxj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uxbkhwfn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rreoiqcy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bwgqnhvz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkneooll.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jofmdjvd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mfgwricq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2soazvhco.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bouzolsr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovewhgnj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ytymqqvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltioilqm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpjzszq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqoprshd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vwnhgonm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2irsymffe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnvmubdk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jgluoexy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hqysylzj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sunxrzpe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ybgmqdph.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lfrhqzki.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jurvuvij.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yubyzuna.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2okdvncso.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xycvgkja.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gccrmain.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nuqiquwr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zcigouxb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmwzvhnj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rgcwehnc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tiicjxgg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quszzvgg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2buevefeh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rcryfzqh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrutxztn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2igyyioiv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sqflfemv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeexvhzb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utltmwck.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhfopyby.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzcqolpt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zrvqlubc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnzirfme.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rfltqbvf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dzezbrvz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bzcecdsu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjuoiijl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qnciqxeg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnsbsevc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xfxvxlmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lzswwylf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dcarhwxx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jxrgmgxa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2akcqqvnu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gueszgsk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivqsqqyr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tkhnftaw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wphllhpa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mtsrxxgt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2suxfhndj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sceynvsr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2upviedpe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2izbtndld.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wjywllqq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2exnbybyt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrbqrwhg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnvzitig.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bjhucami.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bkivjtvd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vjjpuhff.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpowqesf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kdbdbpbo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wfksutis.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yqsajdlx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nujpbyrc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlugwkz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abmrqdgz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kihrllwv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qmbegphp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2emquyaoz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ocqyaomj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tffflmxo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jjdzmrcb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2arivphjz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eyrmqblw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2okxvcofi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2klwpoqka.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rxkxbbts.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jzwivllo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mjmogtyl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mksljvmd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2inqhfwko.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icsoctov.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ybqnslkk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yvuwvhrf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iudsitpz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kpeenbqw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kweeqavo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2eonohenl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rnjzacke.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbyunznw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bkvtnjvt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yzrjflbd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcxfkme.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ntcwukze.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bdvxrgdd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jfftnrnd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxkwponc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qhotgemg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ijuwozzm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tplsultr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nqbyaxkj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fpqcllno.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tryuenzz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cocgmfux.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ggfktzov.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2firsjbat.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xrifemsz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tyxjeawq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lpiosyni.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pxzvjjxu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcbsbqqs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jerrhmwe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ubmdnbif.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dmzhxrlb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mpkjqidm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckgscuul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjsscdko.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hajtzztt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xamqagvu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ejfirldg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wrzovxgi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uvnhgdeg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nktfixic.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yjycuxob.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2diveopfx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rgajknfm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2trcakonw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oiteyjfh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yavxdzmh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xmyinqsw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hdryddwj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bfltigyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awkrhzjc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lrrqppol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlveeedv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2halhlhpx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tlarbxmn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2buqahphq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2onuzkqzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gktxpflz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2abuartnq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rcblghnm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hgprxrjr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cezybocs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jdjwgqeq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2osltolot.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vdvxgdbh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wkpgvpta.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvbecpnt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kncfumzp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2axloezbv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kskzgvdf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fthmycev.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ycnuafwa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zpzmosij.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nofuweaq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mmjuyvgm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tlxeksgb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2owokzzrg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xtmenxac.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2undngsim.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2moajdtfv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gitkrwcw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qpngazdd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uaszkbyh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qxbwfpcu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kndqjpyh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2znbohlri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgmecky.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mafvsfow.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoxocrdp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxiiellz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jxpwwcsf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tuadyjsh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dydrluta.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jlgbrwcs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nznzukrs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wfwybdrv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wgrzuqeq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2busjgnwe.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dxhqglvb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cvkrtjgu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ynifrevm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zqyqmzej.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ohqembhk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2llqeyzbd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yqeqyozp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aokwsqwo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kaokgedv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2yndprgiw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qiiximkt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ecplpihv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gsenzmct.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kitspsvv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wljdlokt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wtlnvgze.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nxzttdab.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ocupnbkh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2feoahhkh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2cailycyg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2augpszlc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ksdaejgj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zqpgcpcj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zqugubdj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wjhxzmtj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qrtzeirw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ivwcllxk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbzqsmdk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jtignhne.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pulygdkx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lqrzytqp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2citeepuh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qijhchys.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pqytlztf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2flpnjiwu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2udhktiol.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zejgvhqs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nnarjemz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ewoyzmjg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wunreerm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rgkovhpj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2oziodgvx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vwvjazqw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zkevhfcs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnblblfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vutnxzkh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jgsipwea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evmnveah.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mrwpnlti.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjokkvje.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lrblgudh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zegpsikr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zxettjvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rzubtnap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2tecmbqsg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2odloaaqd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2svdokwrh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fukrthuq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yijgxrsd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mexqzhmi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wwqbtqrq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gevobmdr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrjsszxt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2oqwxkxeb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ofrnreqt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bhpnrqpn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2liwfbaer.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuajcnvq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zmgnrcpa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xmjhjnhf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dkvpkvpb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tphtkflb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xshtxcue.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bpzubymo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2kvihuehm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gyvktyif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2klxnxaok.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bakzlvpq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2khewwsrn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lymmftnv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mrzueteq.html


<!-- 参考信息 -->