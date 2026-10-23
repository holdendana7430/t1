代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iietrrup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gurtxkeb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfhvvorc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mxvriilb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xbnjupfb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipieckzj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3euaigoeo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wlvqrajj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bvrmljvq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hibkydoh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kbzmtxif.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qniwhhwu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3cxoclepq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mtwjmxem.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzcolspr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fshqzwnq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajjxuynw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csvxduzh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gtrfoqho.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilmppono.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esvsewmg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtaycigb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wtnotdqy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffmpqvmn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3eljpakzb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lherwlgo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmjjpghd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wcklfivt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3anbytgyb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ksjxwsxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gucksqiw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rkeswhpa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qadsurnx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zwczzboe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rqtwijqf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jmnnwiak.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nesctmht.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xsziirwo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vjituomi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uxrbxqys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orxxfpvu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mspgxyoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfkwhfwm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3beajtiwr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3brqbdkxl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zbwuruhp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeohipoo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wseaolgd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bfhgabpo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fetcotat.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kpuemgbd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vhzluxdm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qzxfyojy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tawxkjaj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cepehzra.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvilnbba.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niqtqqcc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrunbnt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwdxsbl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysexzwrd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbcgllsa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nvdnxhzp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mrobtgiz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oakzfkii.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rshtlbww.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bgorxvit.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hlxghtls.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rubeemnv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sjmrjkqw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3noyftucj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3unmdbftd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wzqjafen.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3urliiilm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3khxoyqyd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tffbmhlp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blzhwtcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xihjukkc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tpuoeyvh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xophojnl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3uqidbajs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cpaqnyio.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3beoapblg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3prwmffsp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tocystyl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hbyzfedl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bgvxlxsq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgqfrbdu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zhnuhmgb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3evtgzufc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cjxbddgx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxeyzftc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zdivfepu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxlgvfz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uptmhkzo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mytzkcvm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3sfphlddb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wzuhpofm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3faicmvkm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qrtqqxrf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oekqwora.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gslcpeas.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gdzsigvr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wdempwxj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sddybgnn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kcuawjfh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lboionha.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fqpxiboq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gohncafi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kogjbcta.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jxlxmmgs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kocllwfp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tybpwxyl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jyolakyx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ucaryzqq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wnadlovn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yqpeoesf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wmqfimii.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfhxxdfi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3htcpdmft.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmhgybmw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hhupqkcj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wvldsvxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xloupflh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kfsznswm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3irkulree.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3idvocglc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3psppecdm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xslqacej.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wutegzjl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3buutltyq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3adlncvvp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lmeuuvlx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tgmletrt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pxtjavme.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3likshgpq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvaxmxzv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rafquzxq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gcfskigd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoingevv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mexymagy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rujgmovk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aipknpes.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycxrgene.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jzglwtmp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kgogealz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfnyrlsc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zkwkqsyf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgpbcavy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zvaflshr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3njaeektp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iyjdwkpv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nobjmhvh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qexczgvq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yhhjajnw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vlyyphsr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dcfrxmmn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sdydszlq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lwdmvpmo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3deidpagi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vdwoczvi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3btnftiyv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sqyeyfkv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ycmywrdm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zhrgqoyn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wcalkori.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3effjjoqd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jkhfpbvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dehttudi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3haygtwao.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mljrucef.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3obollflx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecokppst.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yytruryt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3evedrnfu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3pnoqcqdj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3spciwrju.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dzarivel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ievegrkt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ipbczqyc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dwibiggo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qhfqywuf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbtxxfcv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvkogdhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jcyaryjz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bafugxoo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ybopfomt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mhufyrbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npmdjwbs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ngubldch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zpkvtcpz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eunrliyn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3grcxbeja.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhxhmmnx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fljpvyuc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qyckavdp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3logioexx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3metsdmku.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqyteqne.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtxkvzyj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dfrfejqz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lxxaewyr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbbkyofa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpoiccqz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gelqwmei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kpzirkle.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mnuohqga.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gxyzimzj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjkhlfae.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3iuccvouy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3plxxaxpb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3btrygarn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zwjhptbi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ofcagrpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uxthnaps.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tntpjmkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3athjcayx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mlnpnszq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uhygikpw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tjtltivk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xskpubmk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwxgxkxd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnqrtdgr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlsnaqaw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mboazxny.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mhwtnruh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zvlalijk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bicpmfjn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fnjsdske.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iyixxexc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ybdwanif.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3brthiymk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idlxdvmz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fxooekbf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dxbzkjir.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bbpmwohx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ulskuwxk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xcyftsaf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gtpxleaz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yropjmea.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dcivhxnv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qgekyvup.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wazuuoyu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3txuedklp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kpwjdsns.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3npnlnfqs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vmkprsng.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zqqmdozt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcwvsndg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oswwxbdv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hehaxtuw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nbhwlguz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vutxlude.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3twadnzaw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tvtnnlxu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pcerhbvq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bmoyvojs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dkpzqlsz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3itoamclq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3nusezhao.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhqopiz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ukouoviu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3doasmnsv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jzeakjqy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3utjypebc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wzwacixo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mwxcqysz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nissrncc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bldbffbe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ibbwmjqr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gjudtxpo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3olfwvixl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmjowv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3srnqvlwa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kslwjatj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vhdxqvhm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fgmhcmqh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3uupzmqzn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3usezaobe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ymofzwou.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddkxutxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxitioce.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xdrnklka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrfxtlhc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pssycyue.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xktsufpz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnyvkpbv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewsisfdn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmsghipa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3wyttwlzf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3vwqplufi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3svgqahev.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nsakzruz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mqdynsiu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xecdtjfj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vbzyvavl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xfmgpvoi.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3huquoxyy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qteqbgbg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xrmimlat.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bndfzuci.html


<!-- 参考信息 -->