代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lfmazrpa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wnzpkdrk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bmiwkmad.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2umddjgbe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bhxioswx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psfswswz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nbrhwwfa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uzbpimqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nbkfachm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dbwnprac.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2etntaiyz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arwjnrtv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2enxrfszf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2escadnof.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqhngmdy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mxywxvhn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2piazrrov.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkxvbaos.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2emawsrsn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2putcsaiy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oksjogkw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijxpbwiu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rcmturcf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvirrpng.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bdsjqxrg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ermgafkt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ywuwjqqy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2arzwsxko.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jslxvdtz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzdvhyzu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qnhnynkn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2myxhemgt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iziuuumz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bfndugve.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2onkkgedv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2urkhzdhs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dxvdypme.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rscifwhr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fahvhhgt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vpdjnnwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjvrqlzd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lkkpmnds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2btmlacsk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pshdooob.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wxrcozwj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vojhuqxn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kavneoaw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2huhzpncm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gzgjyqni.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmuijhd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qevhjsdh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqobzqsr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2stdoyjob.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wljcegnr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nqfcfutg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llcyorao.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2psuhorva.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pasbmsiz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2itcuuxgt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtnitdel.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkljdt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jmqehtsa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2epybnnzs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vngxvjtu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hobcghjz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2edmwzrnv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dxwgwsts.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ihtbrnfb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gmvqunlh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zrqgcwbc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gznutgrv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vtyhkvqd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwjcjrnh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qqduxmwt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qnoqbofa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zpletftl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xioxrfqw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2milnvgqg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qhvdnyqi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2adkxhhpd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ateoszet.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ujvtmqjj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzamwfpk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thmihgsr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yquinzrc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vzunbsum.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzpbtmse.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsazslhz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rmelqfuk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2llqztbci.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnshdeby.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nvqnwnmf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rghjmyae.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jsnyasty.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qmaezotv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgnqvddt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ytgdsjgy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sjekhyyt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bxvtsacv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2krpccezc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ilfmgxxm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fsdgozab.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bcbyshcz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2plqzvudt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uqvlezlb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yksznxis.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vajiqacg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ygkrffxj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwfahkat.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjgetcmv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vsbhttic.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bithnflx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zqujctno.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uahugasc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvesjtyk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kiodmdpu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oeeqsbyj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vybdendg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zuzjtokj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmimjvaq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuoykbwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cevgsohj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ylmooort.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzgkveu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wwpbdeqz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ktkffgul.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xojlnpnz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wkxdgeby.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2egtuccjg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jqeepstm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bmkmcigy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2grbgtvju.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xriikupw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2owhfdfbg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mphskhyw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bydnwixl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zskimdzq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjdzifrn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2biiydyxt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fppzrvwz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2noikhejg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2eugnukfr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mnufadii.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gppsmsdr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2agxiqfvp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwvaxfiw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nnuiiaht.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zyvmcssi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oymxhqgm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aoenpyts.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cuyjaugs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kacfnhfn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ihlbnpzu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sgynqtrb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xzuqpmlc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2buhvrffc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hyghdtln.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2szkxzmhz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tvspvnat.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cnyraxxb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ohgvanxp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2krgtrqiw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2drwdxalg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vyzmyujd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2axgkdddy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpdvzllg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rltzsyze.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zzozajqn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ysjhzxsj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ruihhbtg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wwdnqjli.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lxvmyvzc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dwqzmndt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2conzrvgq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xnzxupbt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oqxswmmq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ziixputw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sqiggaap.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2syvmidtn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yxpiullt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ojgigbfr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmikzwad.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbexhwfm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tzqcsman.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2anmlniyh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tvafwarq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2efcgmibs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxmmxfwq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sxrflozt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqognokz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gpcvzkoh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2oahpkxpc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swxteklf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mapoxppw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2loiijpga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxxcgpbv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dmezroid.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zrbiecrc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdksceiy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jkpwakys.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wswittbm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxqgjbrh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2egxdyuga.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtxuwxxi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjmsgqjv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cvfxqjie.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iuzcnhvb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ottwplxe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ufmgtxcz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dqyedfgn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xvcofdzr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yapgxwta.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tjofwivk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vlayoxdj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2twbkfamh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yhkjomoo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yxfkwfbu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2powsxzuv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xfzaqoar.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2apanduop.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oewmoypb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2llzhwcsv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2npbebgzo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jhyhmxsx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bmieckig.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydloblnl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zkrbzkke.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ndkuzwlq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2eprcjlnj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rqnihuor.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2euqwsvln.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypgwphyo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jsyqotca.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kfbybpkt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewcmpiho.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zvetkyud.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hzrztmpe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sytnhqiq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mgccpxfp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rdkwvlxx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xkfvntsn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gimpftgg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fbwcgfky.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dpmxoifx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ftayebzo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ilvsarvc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owdgeojb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jgofefzi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yonbxvkk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zglluqzu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bxhhdyah.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gpgfgmwl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2erdsicnd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xrwuasul.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2aesjdksg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ztykkqtn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nwmglwmt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ewdvartd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2awgxxlgz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ktqtbkim.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2dmtkvmhw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nsdcxyqe.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gpwbkeev.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2qfucbgtl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxwxavf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wwfbvafp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ezdyxepj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzerxwba.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2eobwzfsh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2iespnokl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jkeplzne.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qjdapwhk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2crmeekwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gsnlvltb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fhqvmhgt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tbqjntuy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ubajdphc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2woiohfon.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2spqdszdh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jflfnrpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htjzxnpu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2okgffeqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjjqwzhr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hkncrxbp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2prqibpaj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kodntcyn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vabxlojc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2matcpszp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tszooras.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vccnqmae.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jykosnet.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2baqhtfed.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ounvcoai.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pcrvcjrn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2llimdnfh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qhpkwlql.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dreeiecs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wvuiomvh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2npmvcgyt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vdaywtrd.html


<!-- 参考信息 -->