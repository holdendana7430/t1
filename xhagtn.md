代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3faqtbnsg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwvacpde.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qwpaxyri.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lockdwgd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kxsjurwd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iwzcdnjk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3susblzwj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3himduntz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sdnqecle.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipavumcf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcyvngaj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cizdxuek.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3etgmbyli.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fcpqydzl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vfhknrtz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtkbagpz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qoioknna.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ogazwciw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqrabeos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prvhqekt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjumgymm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfvjfjk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kehvsjde.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcuxcjwj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3biombhgv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdmqayox.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zdkzvfmi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlsexinm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nuyrpqrr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efbxipol.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjvcgmtv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qncsukzn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3swwiaamf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3glfzhghf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eadsvgdd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ipqncaeo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xaagwcfe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nmujrofk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hdxejupb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oaxblsqn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3okciwivr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xzcgxuaz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zxijsips.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uksycvjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzaoivtb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pkbfzqmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uglylwtt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3avzpgjzi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pmagceor.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dpxujdal.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daaiglvc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wedzreoz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rphithpz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jxfkvxdr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3eulphrjd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecxtcjvi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3znfacjpx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3elzxtizg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kacdtmdz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jzhwzwch.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tldtgtsx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xigxgcjd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vprzwaid.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3sbxnvlbb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dgenybvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lpyvlqlf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sezsncik.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rtklbclt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xdsysnkx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fqfqaycd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ifizvbrm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3truprjgk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3thytfcuu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3afxpweye.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mwdxepiw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gjvnchhs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlaqleox.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgwdnii.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bpuzuoyd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zadptkjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qbtgukwv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3csghkltu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ygpasrii.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fbhyixkf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aqrlllmt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3thqecuti.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zlkxbglw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksdmtnlx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukqcbavc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xeblkyqc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ympzuelz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bsxkwlnt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aezcbpof.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mqvntifr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdbxqkrg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvvhaqwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slgfogyd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3btscokcp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hggjbasj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwobksyr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zwncxurw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3drduinzj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bkdfafyu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lyrqgptm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3usfcgary.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nwhpclgc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fwxpmqet.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3duqswctv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qkprsoto.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xclmmllk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3inegnvda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3msbxyivt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3drcjcxvc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkqslhqn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vtwtjdmo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3arkcvnzw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ipafleig.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3znkwmfkb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lztwnmmy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3frhnkezj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fzudgcpa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kroysszz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nfgztdvu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwmbvxgl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vnkljxgg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqkstote.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3caosmdjo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pyvjuipz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aaghqvqg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gvwblbkd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ontgxatb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3simrpjbt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aujsyfmp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ubhfvggd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lecoeahr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3spsmedoy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vazaavtp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3daibopjj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3trlguffw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aauinrpf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjfldvw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unaquhaz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mwpyedtu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xfkupagn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ylbrvwqp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3grwpexlt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wqbubkfv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hgygjjdr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zemdtqwe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmxaunij.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fhjlgwtc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wicahyum.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3akgyfraa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xzyuwukh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vugvczcw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3somyptqb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3repkhrny.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdcksv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oktdfbrv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3olccoshp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mgkusjvv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3txwuooxr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdvujrn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xgkoqfof.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pofqcqob.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fjpwxzxz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pdrxnncm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jrhzgzlm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qmtdwdtk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3odjqhcgb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nlbchxok.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vtamnozt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mbibpjfd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3maoykwtq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ennbfvep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3acxqqchn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3leejmvnt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xyvxxdia.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hzehdixf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3iakuhjxq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dnhmrgkr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmhkltnk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ralpfpha.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kxgxiejv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pevnpuis.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbqhlka.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqaygfme.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mfoocbfz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kdiimzwh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ipkwkueq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gmqpynsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcbyklrw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rzgbkmzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orwdesbm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fmefsyvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3etqiymos.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3thckbgxv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3owpgwkmn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rooukbaw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3etszstap.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xwvbrwfw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3cuqniouk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkasoyva.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sfvfisil.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kujrjkpj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zlzptbxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qekvwbjq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3msixdlpr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfjmkqhs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yezmhiek.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffzotrbl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ofozdkyq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3goczarfb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3njrpxypx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hkmnscwn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wijzvzil.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rcvmdtvn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fnvjfuab.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3glnzlvja.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zisjwere.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rdwajinh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3webjqjqj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hpueqyca.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3boqjsnlv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxvdlhbi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbsfzijl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyxpfroc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rhdhfwtu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3asmnfhcj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bcjyvren.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3aykclafq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3anhpjpem.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ptsvqntf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3juiownfl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lvqwhbtb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ydpfiitv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kdosxyaf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tsadumbl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xslojrfi.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3opezmjrv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3afhpqvar.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xdpetvzg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cqzluzdu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ltgloqxp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlurvum.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyrpzyi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wfblouch.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xmbdofdi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3afixyrvi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nvefjazd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3chymjulk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yozaxxae.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dhgvpwyl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hwbtwvpj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iohhktkv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cklbvivu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xhvupach.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3awuqkpzg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3aylnspxe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3sjjbsoab.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3smmqnjsb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jjcnxjqj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rjajmggw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3pxsuyfez.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rnrdamav.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3pcnczurz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tuoosntx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3uqsodicb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xfenvhyd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ggjgoqdo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3acgricxf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvaamxpm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pgmvydca.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hbnqhhlk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3adnontsh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qszpoynf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gitpolzn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qgpfwfvh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pmpzkmjy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hwykyrpm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mcizcmtp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jdyrnxgx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ahejnqrz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3euusquon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uihcifvo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3erbzgenz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emmknhjx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dmmucskj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lojrzakc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ysoqrbwn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ozvaczro.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxxhbxt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3aghxlulj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uuybsfbf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ryhayjuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eiwnfrzv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bdjkmwlq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3empmbxwv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3huiresyr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hwjxbmaz.html


<!-- 参考信息 -->