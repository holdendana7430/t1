代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjjxufwd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahmlzfvb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mjaueabe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yfxzlzhv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yyzctnzp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ssbomwua.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3syertemt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfnuidye.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wjznrdul.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3auxhxzca.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dqvjbrzw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pqkorvto.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtusrbx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mnrzxjck.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fnjcvywf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nkfjjwjm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpmpboa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ligtgbpp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ciuvlcjm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lggdnvhs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ibtdriet.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rznxyqjn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czhqezqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cumuybqb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lkornpug.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wpsttnpi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qartpban.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftfvqzye.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hwyoqtob.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uncudqal.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sualbfyu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jkyvhyrh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slbubols.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tznvdmux.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cghniwzf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mefnglmz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pebkgdms.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbatkoyy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bnymvkwu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqcaaiga.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nphnboux.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqanowfa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3katqduhb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ndmqjuoj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lrsbarzh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqmmidha.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mwemvpgt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zmetbyfo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3grqpefja.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ofbqbrdm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3atrruxbz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xfosonwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xvjcqhie.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vdpmxhbz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pairidnu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3shjfewsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsjrqjqv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3eqlaovom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjaqfyme.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ndasmvin.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fsybmqkr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3sukdjgpf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qjrrjgrr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3remnqfse.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avebwglv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ksmybrwx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rmlfbzbr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmdxjmbx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sktscyiw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qgptuihu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tdifaepg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cmsgvuav.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcqfpnbb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ihozcsmg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3sqyiffcq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hjzwsopq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ttbykdkh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3advcmmxd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qcctgbqe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qshrqayb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pqtdpghq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3onbxsacm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pthutxaj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uvbfxarl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3evkknxgk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zvxvnaez.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ybrsqupk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3psqiwefo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rijvfeuw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3grouhino.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcgcjysi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xtcgetyu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgrpxbm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fgbvhhsu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3addmjpcp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mlrrioil.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nngbciod.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sdzbqnqu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pecmmzry.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmnxmutd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jglxladm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fottjtdi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wagjulez.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zcilldrk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsdjiq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3txpnwchh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmtlmxck.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3izwjdlnm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tqzuizen.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjzqqwgk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gcmuqxrt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwzgjxww.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lexulqfj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ijnzrfhf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zsdekmom.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kolutpdx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vjbklxbp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhfgswia.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3popsybha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wdmkenxl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3axlztcxu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tydzocrt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kwyndomx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3thlrdirh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifqvjumk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpallprr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3aetssklp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xbpaibqt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3yumcluqw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bdrezyfo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xgldeduh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lfvfkqkg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qzzpsvcw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpbdoxl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3weyfqokp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tigxadrk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3geamttne.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3meposhzx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sorojxiv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tbmwxloh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wrrxmhzi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3flncfdju.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bprdiutz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vuhofghg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iwtjmxxq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jyjfiklo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bksehoqr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cytjxixp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cpunnrcu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xnwynpcz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mdmfbfog.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xllcktgk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjlnecfo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nvrkrnui.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ragyhueh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vvkwbwqt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3grpovvtv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3htuhxatd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cimxiuhu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ntapiohr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkngeimc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oexgsuad.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gftndmqj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wmatfzyx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bcwsmcgh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mpotnppb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3relvmign.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qeilgkpl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkwaiqa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wjjyontl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kdvtnybi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rwzbatxd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gllzgfqk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3depfxbid.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3phhbvqpg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gnoxrqvh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hqmekaqc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3plnfxuvt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3icjehnjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3frvhyvoq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rhevevuh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nivanywa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ycicfkna.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uvoqadbb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dcbcmskg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3meurpbgt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3quweigdq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ejdeqvku.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bxkoyyif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jilzbgkh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjrieal.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aflvvylb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cwtqaofe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uftiesyg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zpijarov.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gvxetuay.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hjsxdrvu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwicvxa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3snjgfvwb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tmbtwucy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oovzysza.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3aviktmpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wpzuarrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftybpvid.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ozbzldsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhpsgngn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nagtypst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzetunw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwtjhnr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebnosotu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yqhwdwpw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yijfnlsu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yjvrrsnl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbaybt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hufqzuun.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wcjzquoh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jjiytjip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eezfyfpy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yuwbmztu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnsvxqgn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlchuqcr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dcpyxjyt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3piknqesg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3diybfjrv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fcrekdlq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qqimfvmy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lzasmnhh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mwtayvoa.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bsdpfmis.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3evgatvfl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tujtjlok.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pdulgoks.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvbefpqg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jpqrrvgm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bansshyz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3memrdchq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qpfxrglx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3apveycax.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ebxohyzi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wrrelkql.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xtqlzpnh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyxmnurt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qrfksjbm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yoyaqoai.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gpnzeqgy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hnqdygtg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gpwflild.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltivftlp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzqsebh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dscmpnkn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lvcocjst.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wafcyaip.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3szxqbiyx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sgdftxbq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vwupdtgq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3llxdptwa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dxhphqvj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bthsekpb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bsjpsoqm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aflaodjt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mahshmso.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3avvzydqa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yagskrwl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wwenlolj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dniwmctt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rrpryqva.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jhpqwtze.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bkzyijgy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lmgnoaku.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rslynsyk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hknzgria.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kqwbrdpo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3siiklhne.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gliuhwxj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cewjkstz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hpfvwydi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qhziffoe.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3swezkyns.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yieutqhi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jbbkbfxy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rpxpzczh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xrdxnesc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3lnhjidww.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbxlequy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3soudxqmd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gznfgqvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qdyhpapq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rrisomvy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3vvimoxqu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hjueonlv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tgfgjlip.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qfwgngrr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lilwgkri.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ddoamhgw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjwobpd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ykrwxixq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxipbjiu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hxjtlxjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avmlmghv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tuuxbszo.html


<!-- 参考信息 -->