代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3spzswupu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3amkiopqh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hstkibto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3joxninsb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vrbklslz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3glibbxqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rdodxyrf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eftzvhme.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ejvuefzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3axubjsmu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pcrluwkm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwitezk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnixcxv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3asqtxmqc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wxmwpfps.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lvkltpoh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zdauuvxl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dophhqbu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzdlruho.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uaoikxrp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mamkiafg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yatrwslg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cxpzgali.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlligkdy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cjcocahb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ylrcrjhu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbmkjgod.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ytbpljgp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqbogvwq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsslzymm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fzocspgb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tskrvmhy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kujnokht.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mohdhddz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3abqdnrpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blonomxr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmybabca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtytwbn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epyksmwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3knfmpwah.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ffbfhizp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voymgcpq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3tfcsrqzc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3maxybsfh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gvxzswgc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tkgvmtsu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mxihvvmm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dmchjnea.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ficfpmuo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3poogypmc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ewksklmq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jmajxfxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rushynta.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hajgrolz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seilutjp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zmavdbhf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vjimbhmj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxbxemjy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dirkucin.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3chkqxnyb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3psrxzxsj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dwcmdwve.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iehbjzzh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crwgjuwr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xdqwszrv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3eaqbnoac.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdchrwry.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nndocamu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uxlgexzn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aueeabyh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ifjswwot.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3boioorsa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjovten.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cgvshitx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bxrtdxnz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ljfqhecw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3swtuhloz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3okpxmamk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ailrqsnf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hkqcdnau.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3agdxatxj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jfdbikyb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wglifaxb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3znwjmkdz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qlryzjmf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3palicbiv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tncyxluy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsellcu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uceugpjm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmtrvpci.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vcpilqop.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3louyouzv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gplqrhrd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgxxwequ.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3okhnqszu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gzynuqcd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvnphroq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jwdbipaa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jjnoytil.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bflrgekl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mmozrusd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kznpzxkv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3otciayys.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdkotut.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hcwoirse.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhuuegkn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xzktmjtg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qzpliubk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bxtskfzn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xppxxiee.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3oqkqdbzq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3whqkzhjo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xzqmhyti.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fosszobz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wubzbkvg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ixcdysvc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ozesnjqc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mlcqaxij.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kcxkusuc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3upgenrto.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zyatzimj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pbqvqtqr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ulkclshy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mpjxvawa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tioleofs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tlqqwfvb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3anmjczda.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yqncpemt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rggopdxx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3shghnjhs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jxonxgxo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xonoxjof.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qzynqght.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3grzfxfjj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lfpblvpk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3foebzqzf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xxrxcqbi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xzvxyjye.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3goaunylq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fnqoelia.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ryenscew.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3znopatty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sulqudfc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qizifkab.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iupdhahj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3blhwjnqm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vgecpspq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wotwkkto.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyucqlln.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxndfusp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3onddhpqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bqteymjz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lcddfuil.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3peqpzevk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3byposabr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gshsrexv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3unbbzdtm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eybmksye.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3swicpxmi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pkkmswdi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wotwdmct.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzhgguhi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hqrnmkdd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rhpxbcyk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ctrctvkb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rawxvkrg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gbbtgdqb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zncmmflj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oilkkdyb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xsrrzgnl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xzheuzli.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qwixykni.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3numvpvua.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fwkmzmnk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xvlqjncb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zngikqiy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tdsbmpfr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbivpviu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dhrmjmvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3edqidioi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gvqekoyo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gzirlvbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3odpuvsnb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sodkbvyx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hzcsxfuw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tavovxoh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cozgxbka.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3brcbxtyc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vuhistzq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qbqseuxl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hmrvuwph.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hrtshkdn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3drmmuqvd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fabgwuki.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yoqgxhza.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3urnwmdch.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yrcfilpz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tcxirzlo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ppzhqqsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugtwwdbm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xfbwmugm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eutvyvop.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jblgthbi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cjrndjqe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fpnotbpc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzerkcc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nymhzfwj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zvyksbzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3aehmzkvg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlhktrjl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qginbmpn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3siqiikle.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qciedren.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3arsenwkr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbvatdkf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygrjzscs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ucijyjfx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xnbbwize.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gpfosxam.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3girzxnxz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vxmpllgx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tqbsmzob.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cmpqlzuh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dncsdkea.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqdlanzx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3guwelcpa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmzxut.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cthoxydw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ugqqupqd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kndpjyek.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3crrmwnth.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vdblxwby.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vvwnjfvv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyybnoan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jdcevvlk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wdzauxwa.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfhsciwc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hmsftofg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hkokqxox.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rarajexf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kjgmcvzw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kudcsczw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3anrtotds.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwrxtrpm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zhlxeell.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mdusehrm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3umufwdff.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fluljqrb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ctexxfay.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bqhizaxk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3owfstcsh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ifbgqwxe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3onrdlmzo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhxqbwe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cgjsqwlh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kgqzpbzl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zmahdfxh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3latygqgj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnwbjzwk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtmxoynu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kxgwfkxw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xbxskvdd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lvmapzuv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ukcaevoi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oarelizz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kasgjhpb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mmifzjwh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zpalgvfc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yxlbfvoz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gcwtawqc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3umxkebdo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3stgbrike.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3beemkqzb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gsqetmbd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uhqqzgqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zqnhsxbu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bjlxiruc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3temoxoqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nkzwpztp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3narrtcxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3izweaavt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3veycvvxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ocxtcvvj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3mivygvse.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3umawqgig.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kyhnveai.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yuxklhhf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cxmeaiiv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3uwisnvnj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3omghbwbo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3aqzfonit.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scgrbgzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyrhruqd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ppexyfnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhlqroil.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qieyhjwv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xtuavoyd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3epdsubqd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3limwciby.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owcjtdkb.html


<!-- 参考信息 -->