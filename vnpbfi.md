代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmsspch.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oecmztuk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3razmlqve.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3erurnbws.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3snqplidw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3poesenpl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3glccznxj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3prgfkyjo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ifgyulxi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jvtialqe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yelxfhnd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rgdzhebe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kxbfgxru.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yszukteq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3owcrexlj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qeieswis.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jalzvqoo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fnacewju.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wlfoyjkr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjogcsaa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3birdurww.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kathtkod.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlscvpsn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vtifcidh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dkuqqpko.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gjerccmp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ebiqygfj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aihubnbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xfytphjx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3slvmsmpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smrjgzcy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqzemmuw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekguefsh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3midtuequ.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3foxbaxgj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snzlgzwg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yynjfqvk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlmafymh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3temvtpoa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmdnzxmx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3omiuysxo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejxokicm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obbiajur.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ucorcnlo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vrussuci.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agvcggfe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbqhglzm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mvrigyml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nqpufaqm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qijdyrqr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fkxxkgdh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvhwox.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3defeopxz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3revrqpdj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dpuctrra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nlmmdxzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwiotpyj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ekohjdbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cezyatjx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fqllwuaw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jbtxquxc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vguahbkv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3csrnsnxx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ziqawdeq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhkymryh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pohcmmvf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yyvzeuyl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cfzvucpt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgokwcgq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kouzcbmz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qrppgyor.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaurokdd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zntgadat.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qyxnzgsf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mpakgtpu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3aksvdvha.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgqketyt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hyjhjnpe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3difylnwn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jfqadxmg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oquxnzup.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3piijqkod.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eikisfdu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dmrozxsp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kvonlwno.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qlfackoh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tnoaawap.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fnvoryfz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pkcqwypy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yscszldd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sdggvdpr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3thjcexxc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3liwdqcbl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3igxvhbsf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qscqsjod.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vfymlfee.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zhcvpxeh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ynscipgg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzbetxbm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tanpuzcx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccmnnevu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jybemfgw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xgdcrgyp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3lvrcokcm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3otzroruc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ifvbunzu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iwuuxyrb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ggxbalyh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlonlxja.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owexgxlv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3moodcdzg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qliityoo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rxtmfakq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vizzajag.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xyallwix.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pyfychtb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zcmmubzm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yvzbyehe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3grgtmkgz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mjbkyaax.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tadhlkrb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3unqkblio.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ikaswioq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cosrpmih.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3auuqqpgi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcyfagaz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3coxzcglb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vawwlrbx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wxqaikuo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fggluqyz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwhcduyl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qoivfjhn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lppvadny.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjqqcjz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nqbjswwk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqoazma.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pwtphqoz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3csqbvuop.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ebshunyp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cmnzwpxg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3velzjcnt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mhjqhsnx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pcfteajr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ncgcqcoe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eigfwcwk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cghlfrli.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3evequulm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rvskujwo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bqtzomka.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wxogoivj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdnvba.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qcuzslcu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsayakr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pxlaqmlk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeqsiwem.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bnsmxbym.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lewfrdee.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3basamklc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jggsizlx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qdjjzotc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ziaqvbxv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuopwbsq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oanzhqhf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyomxhrp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aoqeeapj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xctgyyfq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jlgzkfeo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tghdjqzl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lakgekwr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zcavgqjh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nddsaejw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vnrjheot.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rfxkbqit.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wlpszojl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xnspwibl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qlcugstq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3pkoukdsf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3msitxigb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wdijyucx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wespgiwp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dbsboitc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3totxeqnl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvmeift.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pspjpoad.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3udnmckjf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3rwclnvdm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3otzwdrtm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzsviccy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gosnajzv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbwfamu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mepbdsjv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3swpngwal.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3maooxftj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tygltixw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aqodztci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qfpkfvdj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jrpnmrut.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3redtqtlj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rncrorlm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zpybupmh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jasmmpue.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3izxncicd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hmshzvha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eifuolpi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bujkwyfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqqqaexa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bxftcnje.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hmmvnmlk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqdydxlp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaoczjuf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ctwqhvfv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzirlwxn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ijadqpmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3esuxfwoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3smbaywoz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3imwojyxp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3gexydyhj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fykgpxei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zribjmfn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsqyodlx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igpvblho.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nlfhaprn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ofkmcirl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3reweiqyb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3telluolb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vibdezhx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axrcnaav.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qmrsdgdx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnnhxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3spafhnus.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pohjqxxs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hhbxslzx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvhiugla.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3widlahyy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lnkdpnyy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdakgxha.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3omvdhcvd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyocawnc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3thdjlvay.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3dlgrrfgb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3twowoblo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mfwwsubg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hhiullor.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3nzgeknpu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tvuuxsyk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbglrcay.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3abakkapg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tpcprwfn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3agwrcgtf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3imbzfmdu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqfjaexv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rnlydzsz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tomqttcu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bdlzjeft.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zbmoexbr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xojkbshd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlusecg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zjfqvnde.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3csqdnmsn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qaycfxbw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3llcyiwnm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zagdkgyt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xqimxrsg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdgpidvi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbuqjtwx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fwukrryo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3islarqhw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cabqmxan.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lrawncsy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3zizyfdxh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zlkclrqu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ifbvqpdc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pwnxpfal.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gsuruoyr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jjnrejpo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fnxeluou.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmeqwcjs.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3kndvrzcz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gjzvsmlz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tdzewqrc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ztxnkyhv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rqgugany.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ahaeoasi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rfsaxxtz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pnkvoopn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cstkhbew.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fmapgchv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3oskkiazg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bihiwdrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hyvfuyph.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3eskbfowa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ugvxymjh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3oepavpuh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3rnxiiogq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bcpuhojq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewqmzfoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkhcalhw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3sqpwfkth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjbcjfxz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mcdircly.html


<!-- 参考信息 -->