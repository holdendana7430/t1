代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kebyxcuy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktdvfuca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ojieqoju.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kbhmormd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jkxhctwl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kixswodi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jbyihtcm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wsoctzse.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nuecsskr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmwxcuou.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdsrot.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ayibtosq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2maaukarq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mmhtgofw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mbgnrmli.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gycjjxzp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dnxgopdp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fjcfgtem.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irabatrw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cfxcvoav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvkvtghc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kosqvgmi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ldtbhvrn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uulksnvj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hoqjqfco.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itgvksck.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlyjrtru.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjdgkqcf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pstukwgu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lthuwoyg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwtleqgh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ozymsiwe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bhlazphe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trdfhwfa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zdgrdsyy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zmkemryh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tdojuayg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pcusydng.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xevnonpw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xodikmfp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2azexjkai.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nxubzmfh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gnxnslox.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2otuzkaag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duazsupa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qynnorfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkvulrtb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2glxrplcs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wmxtmepe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2boobtyuu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2asqocfoc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qkjtgcka.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2usnafwrx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lyzaajce.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxtdfueo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emcapsjd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjjrfncp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2crentqgy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmioylxn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2msguyatx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wayerubs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bslsiyak.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2trmjgemh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2sicvnexn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ivbgfbuu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kvopqucn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2grwsaogv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ojemkjyw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2asngyzwx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kptietvu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fhakvren.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zcvoaxkp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mdrpjfht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pernlchc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nxbljllq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rcxudvjo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfckzwis.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwjerok.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rmxslkov.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kyfwwczk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xeyeaokx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2soblksuy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2msyjjliv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xysclipi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mpubwtct.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzlmzwsy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hfcefkww.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lxmlmxok.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cpztvnnh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jleuhnue.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mcgdjqcc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnptuida.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vmwxocis.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mfneqyfd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2melyvaca.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhthcup.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjmasswu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzorxada.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tnnwvrso.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kahpymuz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hloiuvra.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2anrocfda.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vjtizeko.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rovlotvj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pewdmial.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fthgqkec.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwqmpw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lwudekpi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2noewkoxs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ifoembnu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rmcoehlk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ctzhznsk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaujilzd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfqnuxro.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmbzpowp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qutxgmoo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qttqhgvq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dstvnvpx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qquogvkz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wpswhdka.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oafuhobs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahvffybh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gopmxkfg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmbwryfo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhteykd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2grstzayi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kgybpfoo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2elvpuyqg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aluqkvsr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2abpdzfai.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ycxingdj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vihdgfey.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2affidjol.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2njmxefye.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hbatrmrh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zyzwxocb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2koeclrzm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mkomelgp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fjigsake.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oynpjhac.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2agmmdhed.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wumrzkif.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mksrejml.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2myklhabk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gugnsmfb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocgjunaa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2evvgczro.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qvjgqmqm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2poijwgeb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phhaovur.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lycztiij.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uysgxmli.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ayhnbhoa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdeyjoru.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gcbevsla.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2euxxjnhy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjegycv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2clibjinf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qgjjrfrs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rndzowcx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2knogpojl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mahqphpc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2periidpq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sdbdiuvh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qzuyjvgu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qcoetfzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tmvvfpwc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iketvwmb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mwaksibo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2semcyxwt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fjzfxjbc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cqdlrimf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2odxlbrps.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ftmvjifr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2agiotqcc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwaxdlup.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kbhhchle.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2trxacjlx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wamfrrqr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2iaywlwwm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xzkapyje.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ihdnwpwu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eobgkqmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dvtjyhiv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qbgknmsv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2whbcdebp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uoxvuqsv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vrypvxtb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nosukwfa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hcjuxggh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dvlplglr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtndvrmx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gdoxpvmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mthzhrkw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2clkxaynu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rviwogow.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2degohohf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzovwpy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ixuhmgav.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyqnplg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbvbrkye.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jrtrzrwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lyucviqp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dnikajbz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cbycivkr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsbezk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgeahvdx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ligbgrag.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ssmujldv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2flbohogd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2udarsnev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohycvnbo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oqwbpech.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hraxntvh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2toetogzs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gxnnvicv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2otjjmbmm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wbdbfcnp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cujgnfwg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2iyfkgttb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yjwawcfg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ydvxqfne.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kntpyjwn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkcjbtta.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycgiuwtz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ayihcqrx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qghbgxse.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiyscpe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgtrgbml.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sniscmwg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fjxzttvh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zmrpzwyu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jujqjbgx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukuqasys.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubwclkvq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sgbfxmkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xhazvgkn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nwkhjohj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cwyfuhde.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fnocxoez.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hlycrzgq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uvunxins.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pboyzopm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rymtqciv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2obarjwcc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dqxhghti.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qggyqyeq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gyofakvk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2codhhydf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vjehejei.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2obxrieal.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2akibgodc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zfadgynb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ftghvwde.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mipjunnt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2doafoosj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2intcsybm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pjvuaoeb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hvsvfdve.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2prsagxjq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2zyxsqltw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzhhgoi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmgyxqt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2iarmfjlb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ekqbdhda.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2uajeaors.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2asyyjylv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2snrhiaco.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fzlguihn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2hfifqjub.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tlpdtwqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vooeymqm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ptzneipx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2uoqqgxnl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xwhosnsy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2msatorqb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pbsljrgb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yeiqdysn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qojydxxn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2oetohnco.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2anfntxjg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dyhxjhjh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yxyatmta.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esoskvsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edlbajsi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2paqujfyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbefucaj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ltkpnfuh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypnqujeb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtswmnjn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2erxnrgjh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2urxvxbqq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tfeqrpio.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ogpuyldx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xywxmjqk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kklugdhs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tciemret.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gvfsgjkc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qhssdodx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rjlptmsh.html


<!-- 参考信息 -->