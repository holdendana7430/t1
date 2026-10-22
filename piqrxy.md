代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lehqyzcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vwyffyoc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qgcpxaaj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qeieqfpv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rqelgsbb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nvgxaecb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dmngscfc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2frjbxrrj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pugvorku.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdhgeetv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pjasforf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2foekxwpc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xrgovvku.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2plluqafm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bryhfose.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fruzzotk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2erqrnghd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wciydsqn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwydgyed.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nkqgsrnj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzpxmmzs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2belyapnq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rbnhllnz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkhnaaou.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwztnffs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezpfllxc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jviesoap.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwovpc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqxlovpi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cslneutk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqhougfx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuflhko.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hqxzfhyf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aimriwpf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fziipbzv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ocqcaydd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tnetdugs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cuaozpdx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pntdvymb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2muygakhz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qkrnestp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wapsqyys.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2annalgqg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2plhqrjiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtyedysn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tmexajks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enbmwzbc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xpxrccik.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gnzslezn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjlrtqdd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwgsgclt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lojveqql.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmmyfeol.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wkzvguyr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kdwvtyqs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2plilkytj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pyufkusj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2podxhbpv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fluttyum.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gzzyeptu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gpagnssi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdufranw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2enobrjsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgnehbcz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtaqyheu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vttgcngm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bmakrmjk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dmbaclaj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gkcmusuj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fgjarzzv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2viqorqnp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2djzrhjzq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qxcpjlmg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hloyolgn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tacsmher.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nieroept.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jikrwsvg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dcdkxhnw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snkhfepw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eivyokag.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yqmyzbss.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddoxazhz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pywlamnz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uocalzpi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tlqysyuk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xjpsuhnu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2afstndta.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dybigqhc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2newsuone.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vpuzddem.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gogrnjin.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2iwuszetu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2knnhwicd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pwrotcjf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2abqxqkcn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fekhkcrf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgvqyjtb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsexilmb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2winxdbbi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zpiyhfcy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vqxstebh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ndqpmxrz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nhlysesi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2asqudjdv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aslprtsn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jfsavvik.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qmfpaacp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nnoxudyg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bicxlmbg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pvyduhnn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kdkzvmji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2brqooxon.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkzkapnj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2knnngunm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfnamjsi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ospbvgxf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hmrbhivb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2akazeola.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kxszgaku.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2supdlafe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xmxyvwrt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2viuouicu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xgkmglrr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmqefair.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ikcyayki.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2llxxfygm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hoxguydw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aqzuulhi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kctkqmij.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vkkbntbf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jjuyyjbh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pjwsqxyi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kzxqtbaw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ffqejzdd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2idhesrvk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wvdsafgo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uytervzq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2oxsasdty.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jmcsgwlx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgiwtxxp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okkmvfti.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uexciane.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oraejnua.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bsklhxpk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xkxmgdte.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2glepkcpi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wescssok.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ilwbjnkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zilwbvqf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qubtleif.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqbglflf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mixwtvdl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dywlszln.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mqmptzjw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vvzgvkqc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qgmmxhyg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dityeprd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qmtasahk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gfoinoop.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nypgntpe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnkkcmmc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2otbbyqfm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kovvruga.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bisoeeoo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ihxovnkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fbjuqcxk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lepgccrj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2godbslrd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xvkjuare.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cmyebjiz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2taclmazw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hxjlvsdi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2msrxwzaw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bweoarrm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wmpvzibq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2worvawot.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bygxymnb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zpqcwqgw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2toqqugsk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rplrotmg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wtxvwgam.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2liqmosqk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2brgiqivn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2igpwztsh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2elkecnbj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjpjajay.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2whtnfvtz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zbmnsbbk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2plsppvkf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2evvppkpi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ovvwxtoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enzyckva.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tnalczfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apycuweu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xxznuizf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wyvivjrt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ylccydzo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycxrkznq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2klbnlhqf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2isdqcstv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ahjxfmvn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cualgzlx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fymsmnlz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2feihsjau.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2onftypib.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpgaltm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zshjxhqf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkhsufop.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmwtgel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rzstores.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxmrjkwt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbelwhqf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jerceirz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2heqfiojt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ydzgdowk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zwqhdmsp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2odurvlpr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tjotrjkq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jvsiohya.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oldqnamu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lguantep.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qwqlfxpv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2arozaujk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zkwqxxug.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2oqndptlr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2aukpjncl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lbkkddwv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2txpabgny.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvxrvjpn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2doidvknq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2krimtxbi.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qqzjjipt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2oupzjxgg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2izzgzotn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wazunzio.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dryewliz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwycxff.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jhndgnnx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rxwaygaz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mafectfo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2nxovtgen.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vqixmayp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mxiqtffs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jumtrpco.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2clgggiko.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ypoilzci.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ffkurksi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xtlvpcvx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mtiabggs.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2sbxcogph.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ptukenha.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hogupheq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcasvbqh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gjcphgtm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qtsloxsa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2eachoohc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oapaagkd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2dqnwjfjj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kfxvryls.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yhglxqph.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2fbblfsfa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lvscypnv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uoczgryh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nylxtoul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qyrorphb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2iozvqkle.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vivizmrv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2keetgdox.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rtwoicxp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2khwkaiqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2oyhiepvv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ldueepoe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qdhoihwi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nnxjcgdt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hctwnlju.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ixatesvx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2oghucfqi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wufrhspq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vtgtmcug.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zerryuza.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2stdclsxd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mnnfvyuw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oyluhrze.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ettgklit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlnaqgcx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bkptizws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnxttcue.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2orwdzozi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2aveydwpc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2avheqgyh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zmysuxml.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kcamjdma.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jejgvbzh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ldqdfxow.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxjhiuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kbdgbifi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fvuhwkov.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozyzdrpj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wgyfpvnx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ryovbbyc.html


<!-- 参考信息 -->