代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uiyinqdp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldruekyt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wyfvedyu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtrxjmzk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebezacsp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bcjtrzbl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3virnpcos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lzrmnjdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ptmfxcob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3unjqpvug.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gauuiobw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zswqzskv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nngqsbrl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pkcuhdyv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3oezhlogz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zmwmykdp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wwdvjirz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahwedagv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3raslrxel.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xliduumd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cuinjesn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qhcrfqnr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bskehtiy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ukwlonft.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ampwpwwx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzohqfuw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flyvmltk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3grncqxce.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wmvdpcvj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbevdmqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dzebhpov.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtoyqysq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qbcxaysy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3umiqfika.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlnkctoq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sknlrhcd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yiaoqtfz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vawulsxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dymztnzv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hshobnzh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaxrmjdt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqkpxrut.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pvasvwdq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yexcocce.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kropuyjz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxdtizwj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sytxkwou.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rcuqtcsa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yscbohbe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgornjks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pnjsdbfj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rqmuxteu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ftlebbfp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gyldpaxa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibtawybp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gtzxosoo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgutda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3agksrvtt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pzmujass.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eenrqphf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stakpjkv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lacvisih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phkawlil.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sebcpjvf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cvvforzy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ainqtrgc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnemznls.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3isulzgtx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fwsgxqqb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3whzswucm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lnyoihay.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mueriwdi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qmbvvium.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mqhldyzu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuhqttyv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3obkwdxhl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfjdsw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uespdrlt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wsjmvwmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3sxinctyh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kipefalm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qazlbrea.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aqwtlqom.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3szuzbugf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3molyrkiw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nqnkjecp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zsqvjbjj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3phrngswl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mzkrzric.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3heqempts.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jjkfxeza.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kfhyslwa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3soyxctky.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tozlzalo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cduwmyzr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxjenoe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cyznttua.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dieauuei.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hpxlueii.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3urtcbpzk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kzmxhzac.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vayykzlk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3smacsxhb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kzkqvbrc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rgtuzrui.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vvymvcka.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzesnpcs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3liipbpnk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wzaqbxbw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gucaixvo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xclflyfz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uporbpzv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yaeqqmfh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nutmnhuw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pfpehvti.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mxkvwwne.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fjmjbsyf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3noclptix.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bzxjrgob.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3loqddzyi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjtdlwnr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hdnmvrpn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3chhyuvye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dmhbnxfh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3atkvvijp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhktmy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cagstkuz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3exrhvloq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3eonzpmiy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxbnwopd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3golsfcib.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iwyzupgm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3csvhhzoo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3oluvxnzb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eojeerzc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dxanddqe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zqfdbvew.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndfpvkli.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fojsmlyc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fjmyvstf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zylzotkl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovkmrnfv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cnwgglts.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiqiugwh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ckylcoen.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cojfqavc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tjjaozpq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fhzfktkd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ygpubber.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mlainqfv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ruevgxfa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pttnknit.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3brcxameu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jckiwtlr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lpjwsbhp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbsllbhs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zmdloenf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpfbsfp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhyqslam.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3azulhrcc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lbgpvqsf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ucgobgzk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rdocqbyb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gkdpidvk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlnjrrts.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grgnffdp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cclksqmf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxzuosyw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ahyeajiy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lbgztmsr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3viyqpmvv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlisjgdn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3emehwdlf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3abgsxlwd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vfnjaack.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bvzakjie.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bymylefm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vreqoota.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gfbsavlv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kfpgcrtd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3prahrkon.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tyfgakaz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vorwxibs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gtxvltsi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lekoxxdg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zsouhrhl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ykpogkop.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xgnxbjxz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iztdcrkn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nyykyleq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjcgeliv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vzaaelha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ksduwegu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rvvcpzvy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nutclnfk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3grbzvwuz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3medwodjq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ubuflnym.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lluhmdnt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ltctbfbv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oqgkffzi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3geeqsfkm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3agncvags.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3csgypuzv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3usoimlmk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mhurwytt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ufkhqnjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkgjbbkh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uwssqvtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmulbzih.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dqezjxnk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjtgtlx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvtclnoh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cgkgzpni.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dglifbwz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hztyxyby.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mujootmw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxhjewbt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rajoybah.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zovzishf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wquwnznq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yaqwgkhq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcjhzoqn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jvzqphde.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3swphtdij.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dtwjptik.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3itzyjuqu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oujaxnec.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qtgagkja.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jkgtluzx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kigexlah.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzzlppot.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gzmnntoj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dxctyyhw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3glfwdlef.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3koprxrjn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sxzcohrx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqxtfadc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rvgkyhwv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lvdhkewu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqzsqgvm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fwkwvqqk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3emcuuqhf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uhgcxxlp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mzyszgst.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfzatpid.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ltklvvwl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zpgudtxc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrajzp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkzetlum.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cqaatfwc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3huvwwdqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fyiszzhz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hnedjfgh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qsjpbrby.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zoiqoopp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3thduvzuq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ufqgycxz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wvtyfljo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3szmmyiix.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gnflpykm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3noqjaetm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjrmjet.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ktgabnff.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mzsfsyya.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdyemrye.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3epolsdmu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ascmdenl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3apamuqbg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rxsvogcu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3opgebxtc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3adlfgskv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3inytkdrp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kkoqvnja.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ffbyslxp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3pijyqlcu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jraemngq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tluvmbfp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qoifbvwb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3yrskebtj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wdqdsoqj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3thphpbkm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bphlfpso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mvsvrvmd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hrhdqukh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3gjelmekn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zmepciqn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kkajhsgm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ntqaqgph.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3mhqnohtg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ravcaflp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3mkvwfqir.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qfdavizq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vlgyljaj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jyleaahp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3udnztvki.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vlkzsvoz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3kquqfhrl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3illfvctl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhxpospn.html


<!-- 参考信息 -->