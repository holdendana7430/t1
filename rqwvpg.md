代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3teblhoup.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuutxadl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3oegvvelz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aogrvtgy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzefrhfj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qniscwpv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkdnbwrj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3drffanmv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxfllhah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrqiqhvk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvjozgzt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cgeztknv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ifztikdh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pikrjwfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvnsvlpf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oyglbpqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgmpuez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tczkgaws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jumxtpey.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xmkwtepa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vsevbtdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mmtztuth.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rqbychgb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dpjwueyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnulkzan.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3aflpkdye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpuvzzgo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3arilvyjz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fygdvyis.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wehmaqwp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ujfrzota.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dfjmmnju.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnhvtzfv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ibccevpw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jvammobr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pbkiljbi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dltkbmdt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zicuhhit.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgwnrpxn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvsqbav.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmyeaejt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldzgwkjt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gjwtiqaf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3epktztla.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wdgzrbsz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bkcadwwi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vzojpmts.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fcldwejz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmsexsuh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ahrfofzy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zlallpxk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xnscthmz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3aiqdamqy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kwzcpoab.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kgeeybce.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ziymielv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ywojkrqe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iguxtmcb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fpiebvja.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtfmrjwq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ewghgfsw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxfiadwr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lzznhenp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zvpqswwz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3avcykznd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3leqllepd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bkmnhqdt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3udslgysg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3avyjsswc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nvmdnzbs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xqkvmekh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsbyhnve.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ysjbrwmx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cyxhqhym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuvnpyxt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dielmkwj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdvomkcf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iklrbyzf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uxgflhyf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3joqercel.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3sjnoerdw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gsqhdxkr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mgnydtvb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dynveaye.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3elcimlkj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjdldycr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dztxbsrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3slkddvdo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sjemlofm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mlspkrdk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vabdoiay.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hkyqytwk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3atehuoyk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ihombmuv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gwenywpg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mjuicqll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qsivmyil.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zrfzynyi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbbztkjk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3snbwiakb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ysnyvyrf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3eooevaml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pwbgoejp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtklradg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucvosxaq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kmstbsty.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3evwvjqav.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3myqvngom.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vrxzpimc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3voqloogv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sckghtcw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wgjcgwll.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcncaj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rpomxuyj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bxtrzenn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bqeabzyx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3opyppzxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ujedjvja.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hshhbyih.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kuznxkui.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tkgoxyxx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wilhwdds.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ryugdeis.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nbprtihn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qzeytjjp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzumxooz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngzzvnvg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3baequajl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bwcihutu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihrbgweh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xyvacqan.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fxrhbmhm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zzuzsadk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gzykolng.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ydkxqeuf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kdmwjmpw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3crttfmdw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vscbwykh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ulruymhc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3axjcyqnb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ksfktxxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zattobxe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mdecupep.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jdhyvokf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xpifacls.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lehhejdc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fiznbwyi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kykszgww.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iylqoqoc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbthznlt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nosmkbfc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mzfxipga.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lvhpfkqw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gmbqqrye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uuildqav.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyvytreq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3abyfdloi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wgacfqqi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ocfxindc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ovawmzwf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3whmrcvno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lygxugqx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wqtcpuxh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rkdpxwvl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fcrlrxad.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjbbrjdm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbfjdslp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fmlwmykb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3miqyjrsw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xqcumcib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vnraesfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzfwbbtj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vlsujamd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emkcyvbm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3haleuvdj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gqyejuts.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rununrqx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqiihaxk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kckvmhuk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsnlhjcq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3posfnbvl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wzeetwjv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzunumwn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hhpvlksl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zsoievih.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zolnhsku.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsndfvfa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sxifezns.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ydqkrnef.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3izlvhbfl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvbdhoje.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dusbqqkt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3srtolgsy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wszzhvhb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rrxjrnzv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gcehhkut.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mpyuuevx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3effzdgas.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jesqmsox.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ovwdymbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vnskekml.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vjbkyfqf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fvarkhko.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3etcbnvdg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpyhicrw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzxoklkv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mdmnosyz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmcjnlu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bnffgnnd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3payrjxks.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbrzcypx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zifyzdfm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nyajmozm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xzwffgdt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3owkhapta.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jbijdbgo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rpmyomdx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3taddddes.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuezlfmm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3uyzditii.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3etpenstb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3syshboyi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pcatpgau.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bmqkkswh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lbczkgre.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ottzircj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3slorbupe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ywmwskrw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nafxwlgu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lndmahzw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bhxrdozi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wibargpz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oibaqfpq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3epvvwjhl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nhpimrtf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3icxjyzyt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ljiggeom.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fnayraic.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qkmtqxxa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3scspfpbl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dwwaleuv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlocjdh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wtwenxgq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hrvuldft.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3pcylwghc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3timtfcft.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3llunkwui.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jnfmrnsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3qfprbeec.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3evptwdke.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljievevs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ttvojlvs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bqihlfst.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbmhkxc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3otebzfjk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3sjnecaza.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3anvxhtro.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3opnesxst.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xbfgchre.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vhrdambn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3guxsxnxh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jsszkueb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3iatatyak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apieqpfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoovfbab.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3orosuuqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqxjussu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ppyzacfq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3amqhcnye.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lnpfcjsq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwmiupdc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qvpcswru.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kvjzaota.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3nubfbgyy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3geamooid.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjtonrv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3cdwtadrb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gskptykg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dnllccil.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3foangsxi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bwktmcpn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fpblxtwe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbqleuwa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ndqdmibg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nzykgspi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3szsmnbrf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3yawbazod.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qehrpbyv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xqceviww.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wedrwpvb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rpfuzfbu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kxkegjvp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iipitnwo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rzxymnbq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wfxnjvoj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3yqwrvoej.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dvtlghki.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lzksnzpm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3plrsnaie.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fdeteiks.html


<!-- 参考信息 -->