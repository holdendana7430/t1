代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wclulrtr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ladwhuvy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fphvramx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gbygecds.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2licumyhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efcpzhff.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gobqljgr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qybxagpf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gqktnshs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lqgqinqj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdgvnovv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hboercuc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwemhqqb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awqkylgh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2epjbnukj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jugxlicc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udsogibf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdjkofco.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxjbvaok.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpgcdoid.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcdqgvjk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfaxzjon.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvwebult.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ahycojwp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fuezmlgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jefrxqos.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2eayhryxr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ozmpgglq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uuenclep.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mgprsjde.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zorrwbda.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tiavbesa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2apanuliy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rhbgwrdx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2khknvwgz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2luxopxhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ladsesfn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vzyazhvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqnrjdnp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qyykihfd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ggfempeq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rmnvttzv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lqwwyhpm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fxhyrngg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2moaynkmr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcvobhd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qzrqriba.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjbmijxu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2elqdiqcw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2eruyeboh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njvqxqyu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pviubqaf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2swnwkgzu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2thybwuhu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qovnpxps.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfldtefg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efnnhvgq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gbtnwtvh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kucrizdb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zszactjm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yaegyhwo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nrbqjmvc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2diotbsxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dnfjbqod.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gfgazfqr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2szebgqrx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wsaevzzp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2faukwbvw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dunetiaf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jyscbvyv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vhfuqdvg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzkpzvgs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2unzckvcz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zerphdqr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rlouavvt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xjsbhtsp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wstjjrmx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qynkiayq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hhnclzlo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsowcxsc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2geniplbt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2drwhkorc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2okbtcjuw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zmescxyo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xiybbggr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jfdvftzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bqxaodnd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fowdcjcs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2waebkros.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2poltpoex.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2beayduew.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2goxmmeol.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fotyiucj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nncspgjj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqwtvik.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mztsnksn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oeheydjs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ocxhwynk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wobipmam.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cppaoitn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qbntnbom.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hlbdseyq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xjffrlex.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eetisian.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gkkcbkjg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zvhhpnlj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2muoxzmon.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgtlvpfl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2drjthcoq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2seehamow.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2txiycewg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vfpfcttp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2calhfqnk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfqwndrp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uwtskree.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hbriscre.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2oikqezpe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wymaqnpc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mtmlnzwe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zmbzvwqa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pxzxyivp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wjffupfc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ktayryeo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2stkooxys.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sykvcgtr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jkawqupz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tztyizzs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ozmgeayn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hamkdzfb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dvkgoapk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2feegvozd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueakdnzi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ydlbyffp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2divdjfqy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dglmhzda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hgtrpmom.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vtekkurg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2saepirab.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xrgmciku.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fiqgsiwo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ogufmang.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qcnohggq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zsyzffko.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrmatfp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vtkffifw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nmuirzlp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ddalvaod.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bzzllqfa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhfccrx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kavkbrdh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2scdhkust.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gwityhxv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fwxfbxyq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xmuishqs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxnkenj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2njaywfjq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ogkxxjra.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rulrawvi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2evzdwyks.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ixrgnugv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qkiuhqje.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlojghtm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xdasxznf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jtijfnkg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2txnoytzo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tqcnvolz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2unqwpudf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbpiavzr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lnbavyyy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sanmszef.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2whnbeswr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ifltmyit.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xvctcqxk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqifllsl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tuqjfcrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2czyhmvxb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fftldzzi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxsjxojw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wiqoqghv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2exujaizc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hzososfz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qkqnbjob.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2prlajdwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdyegrdh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2parqrxla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpfsstxy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fyehunra.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2noptyvuq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2sjyfscjd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rdbbleos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujepgglm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wemjptbg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nbvhsqmw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2voqxyzxq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cibmxkze.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pehhvkkk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dtzvtisx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djswpwzk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jslbntbw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwcjtu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2opultcmc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zbggqfei.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxxqrfks.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxuzknh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ymuimxlu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wxejsvai.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gylfumjt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qxhhtdjh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2opmjqvmo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2naufqskw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gymhfdxh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mmaefkvk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vefkudvd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ufxmsfos.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ahidwurv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2enfacgps.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2benotbzg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rknxmacu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxfasqed.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2sqxjgyoy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2chhmlhpz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xummsoen.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2sxxrxxsx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wgeunyik.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wtgbgqhw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lylvcikr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhadxgcz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qkfecjzt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2svfspenr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vxpkbdwm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uotozgqf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bpuzhqpu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hybkgcqf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2evolqdwg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bhvrbizk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2trgjgyoe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qqrygomz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2alfkukdx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ynleltvp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qtohrfmx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2czyhkynm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2lxqyzvzi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swgrhzta.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2efplkwqd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rnbeudbg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rgiylilw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xjlamsrk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wtjzifyx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxqycxuh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zwjpjvzl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2apuzhjgd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2zhfqaopx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2etyiblrc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2drkeejca.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gtlcmxwo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2buicuiyj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hnhpqflz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fcvewpph.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2nclawkys.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vghwvrrp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2osalwhwn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ynvwlnmy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzffxam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcocpfix.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpojbo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2sjtnhcnf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gvhglfuy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gsfdcwhc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xwxgckde.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rhriybdc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bdfflmgp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tnahihis.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hyvlwnhu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2izrmufbq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vfobotll.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ffwqlbrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrzijiiv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vmfprtjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cysruocu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wooykxll.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwcjwkgx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2elnrvlxw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2egvdjaps.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dekqumez.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2eayertei.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sepwrjlu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2giwabktl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2txeauwgp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wkkimyvf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tezhtykd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zbznzeev.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nmjlzhxq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrqeesm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2smgfhibz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wnwwgbsb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jrjruhfz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hevfvzvi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2eikjgdwf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtctsepm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cvshjptp.html


<!-- 参考信息 -->