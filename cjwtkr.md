代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjdqkxsu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lnvmrmpf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wqhbyzat.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qaotgbtx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tfibzzyc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zbjlohwz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cptdjiwp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3etjxvqme.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kjkibliy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dzptpzpz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zaiepxwe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bxpxqshp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qrbscyug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjfpqxgv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jnpinizv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3phwkjusz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3awpgbyls.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ffphzufq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nujnnvmg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3oailwuuf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ijamyyzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksgljrgl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qiyjgkcb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yjmorxne.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hlkucjph.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqefdmky.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vtweybia.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3engpbtgm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ydteswcw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ckbzqcrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3marxauio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ofwsstho.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrscllxi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwcxbubz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kwsdflyh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzykwmoh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3piggitjm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plihzjgq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zudxnqjs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxyfrjwg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejouupcy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnnfqyhq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqxhuxrh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdiuoan.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wiosuoay.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytlefaxx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ehysvfic.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bfxgexia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cvnjfcth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3evvtisko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tijzjeet.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qsynfhjv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vcfvhyxz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rwyhcfoh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dasecqpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3etqvkbqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fuuepykp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bopwyknb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdanptqc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bdwjnhgm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ecltemol.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hqzgnkpm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tftkcezm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzyoylh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rhgoykmn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3odxdoruw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bcjlqzsp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sibjyiqe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fgunvcaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qxtkaphh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rbibjruq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovdcjlrg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vofjvfiv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hpftcelu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ccktfnya.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wadrcnro.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rbockcvp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wqoygxvx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3glczmrgd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zbobfrzw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kxdznnue.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wvdxfozi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3obfczwnm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hjnnrpkk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yqfixpke.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3smjbzmlr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zgzrgtkz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gjhetmrd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmjqbdd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dndgbsbn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iqnjtchm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyypsbex.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bsnkbyto.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3grjvajmo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mnmpfunk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zfuzpzgz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yzoioynq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvxnzudo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zceozhhq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thkobfdq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jodivupi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yresdura.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qreeqlfa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yfyyoggf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qbmxsfqw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3czflqejk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rgqpwfch.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvolsmjl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdlawhoq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mloybfih.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cudjfmra.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wkptfqtz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qrctyisp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ebhadrom.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wnhsjxjy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gapydcrh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vpbygqio.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjlnpwzi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kwpqohfc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ukocxifv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hmgsskzk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bpmdzmvo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qvjisckm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pvptltcp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zufpodhv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfavglga.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gbopoxpm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3eylsydmc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rbasivbs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dbpirjkd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwbcqwua.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wijppqad.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tifmcivj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3igzstquv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wibzsgkb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxptiyax.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lufgdioh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bxywmyfb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rmxgmgec.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xgkgnzxe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wcccbpgl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3brsrytts.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rsunmrzm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ramwxyoy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tfcshxab.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qczvfbbi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nwwbzmac.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fkdpdtwm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wkkjlpig.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pmvxhlbk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nvpmevdq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3etnvcxnq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lbethniy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyeaftrm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wopjfyao.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nayyqneb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tllarysp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ddamymgt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ijeemoqp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kdohoxtb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nijpascn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awnamnqe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjejzfk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qatptfdd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cwlwdrtn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3elsmdlbl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aimpegte.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ktzcrmmo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3iocstfcm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3npmfzvjn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xmomqllp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rfirnqwh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3risdbirp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qtellhmw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rjqoaxeq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3sepppmtn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mzsjijye.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rjoehzqh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3okirrbio.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hiojywaq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3uvwdmcfo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oabcseln.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qglvsfza.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dgzfhxdb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3itmhseud.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ntyhvouq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wyjggqna.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urzdcncu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bqlycxhy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3daycihyu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bvorevkl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dyudzdcg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3aqelrmrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3avkmmrde.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3edeojcrp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wkfxdbwg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vqtaasfb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhycobrc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzneaas.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3doviktko.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kgxqkvue.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rayqsssp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3orivuiyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djbqzmfw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3aebisrtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfcaboaw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bctqhoum.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nqizyqeu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3dozeaotq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbxvhinq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gnkygwan.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xnndyftp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3segsaynd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gybmlffv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mvogzdsx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rnywbbcg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wsbpcwar.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xklknsmq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3llgmdeuh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ykcrfedd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hqtccauk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bgutjrbq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ucqnpuff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytjsnqfs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tgkfvxpu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gqfspohw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mcwysnpz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkanwnld.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3duqckdlm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qiinpzcc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3eflyhphm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nasfedsj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ssixzprv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gkhlvapk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3inhjwvgf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hndoubhc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtwracth.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hapqxvsa.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yxwnnoyl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dbuzixlw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vicyggtj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3euvytuzj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3alsmqocp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zhgkxnqo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rcmdmswt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhrrjiiu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3miinauky.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwwhdpeg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfprnpa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cieghhdc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rtxmtpxd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gkvfsmii.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tqkzwjhq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpkabp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zewfinwd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yjmgbcnd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hjzmyjdl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ajpregkc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jhczgekx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yggmmqom.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rycytowp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3voiatnao.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qpshdank.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bibdsdtv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnfxrsl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hfyoties.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yggzayav.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kejjkptn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hjtxcmon.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hiuhrdkt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bwojtmhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ombezwjw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hkkfrngz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oodrywtm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ijhobiho.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wkqicnlp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dgoyqshy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dcbzazfx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zjltsnre.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rksolfgg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3khijvfyb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3yryjfrzx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3bfaybsha.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3eksxpekk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vjtmkkyg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqrwmt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3oknyptyb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ccvppvsf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3hrbgntxi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3bzaczzqo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vnqjmhqm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pajzyjuc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3izfxnzoa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xqjjxgfy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3nmxinyxb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owvoavxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldxkmlmb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3abjrwtjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwoaeekw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aewvijgh.html


<!-- 参考信息 -->