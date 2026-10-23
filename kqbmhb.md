代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mchldujk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtuzoxw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gboelimw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3svpibulb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iayktpay.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zyttyzan.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zfmlsxom.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vboqblfx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3odtfnnbp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hrkzzqkv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzulgemp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uynyhrdt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzrniryf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmqnivlp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3extswmop.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uresudtw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gafpxnme.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svodtycy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3whvviepm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugfrbved.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jyrjgzth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rufitbao.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfbmknss.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtmcqgn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3urmnlgin.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xodinvci.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3htmgeauq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rwlhobsr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qelxemcc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kyadsauz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tcianbcl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pjwaunnk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iwuoozlb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ngtglpdl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kxlakadd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yuvakico.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aatzgbbc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmitpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzzddaey.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3chuuxdvm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wlmztxvq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnofkxdw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hghhvyzj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3avpwjgwf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgllacgd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dsaezuzp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mihwfvym.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzsqrmwc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ygzsdfdh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nuevzgyc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ednqdrko.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfcpkxfl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fwpbabwk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3obnrwelr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ujkhjysr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hloqwpfq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yytezyim.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3konrqtxh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ujziyatz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wocqfysz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hrqrbchy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lgmfoaps.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mygujxsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kwxrcbjp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wdlvpyzk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xsozzhzf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ajklhuel.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sziilmww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uryxxmmz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3giyrlgjn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jaxzhtft.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivopsyul.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ssgjymew.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xdxzdknq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dtqiwsme.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uqiqwebm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bimouono.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fgcsctmc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jrfcjczl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ofyuvhgs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zaqdrfwi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3udghhsia.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lamgeeis.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wjlybxzl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wewjpklt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hlttlfjg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gljwdaqm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oyltxftb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbghtlob.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qblkypfq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yjyecrmk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3oxdlpiqh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jkyqovca.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rwxmexqz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3obfqvrpx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zffswjdl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xevpzqsu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jpffyjtp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wsmrmrhj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3faembdhk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3awqdjqjn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wgseuewt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lzlxddjj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cpvzyzie.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bntlmgrk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dlnpmyft.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhdgqleo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jauljpti.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kyoyicnc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zfphflnx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uljwgsex.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pbmqfcol.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pqlofzjr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmbanex.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ajspukuz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuuyujcq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brqcikgl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rnkutdoy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oppdksqy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qryfyehb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3miwhyudt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ccvglopp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uxvnruba.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3iyuqlpgi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3snnjntlq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nuwtrusr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oqjnkqdm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xnhgnmdw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mqktuvmz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3riropzpy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zntsvqgm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hamufyxj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xpfoekzc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xpagqann.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rlgmeeyy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aevkipji.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ilbuujbq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ubefnfor.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mfuttwax.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xaysbkjh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ylbfegzt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hprmryir.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sftqfsbv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucecvsjs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kjzmjbio.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3odhkcaea.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bosmcdrm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhurxfop.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzixsag.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bedtkzqo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epzdttvl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3klvnecob.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wheunrmo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ddnvtwue.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnejwuh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3phfvyndb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ogmvscpf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dgrtjkgg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lraigszr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zvcfxqez.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zozacywt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cumflrtv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vskhwprm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nieimvsb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jffcxihn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3onjuskml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zsjqoibk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbeckdn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3irpdpstb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cotztntu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lqeciscf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eusnngrn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gajythld.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3plfcxsio.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lppoqynv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cyklwosv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3seceixtl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ziakbqvd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvejvwh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wruvxucx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lnuaginq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gbhqphka.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xngywqzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ridnrmfl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcjkekco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpwnplje.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ygisaadd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dapocpmw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbynpwhr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkddbegs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3delrxrna.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfagrtzh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kmuuwyoi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3caohbuyq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjubjtjm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3pkslzsdh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cfijpfwz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxoigdlv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wxafgqhx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3opjgfyln.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgovqkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3phydqvcn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mijiqbbd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xrijlsxj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hfmeeefx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wezheujy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mlzqtamt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3amnrcigl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3slrncvor.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lwrfjuxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fgnagtic.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gvxupufo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zuxjskqv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3aioydmdb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rbfbhksg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hpjuhdge.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fotfdqgh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ksxaihvo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3obejlktw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ouqzihvf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjqgctmg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptlgbrek.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3edsxmmup.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3saczhouz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3xzeuglec.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oakdzwti.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3enysnygp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bxtekqaj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhrxddd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qjgebotf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qdvzeqwk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3piscmrqi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3iwbyhfwr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3atiukeds.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3shzrxwcp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3unzbskxq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxoawld.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qmwkluta.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ilxrarjd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vegllkmm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3sqicjeky.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3kawuigqk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3todfkeaz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tiughfdm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zzmualco.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qyzqjjlb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xvuhezep.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zksttzfa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjmrnvlw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bylrhegq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3dtbehoja.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rwciunul.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3srzvmopu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3javxuejp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zxouljyo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kfsopndl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fvrbxbop.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dukxgspb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xuhulzbx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3khwoezcc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lbvoxuzl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dpsglzis.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohdkwwzp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dzcszgbx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nyszgcls.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ndawkowl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nwihxbhj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xdwihuwv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xmuisjuv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rhlfxknv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hgufitki.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3aflcylpo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rqijpxqj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pmbdktfs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ssvwuljv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hugfffgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxbtqncs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dbmwrktw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfetvqto.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3kzjphqxx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3skyzqrpm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3akpxsfiw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khimxkpr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yddvztuw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pnuinxzl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qditjvdi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aqgwhobq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bxblvuio.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ztseqggk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jrtljncq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hofajiho.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3usxdjgcd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxhwxbk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrhgjvfm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvukzjon.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtvmiir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qccukphw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3eodfaleb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3dvyjuryr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rlncwhyq.html


<!-- 参考信息 -->