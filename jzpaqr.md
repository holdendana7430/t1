代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwezjubx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvstcvjk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ziemwlyk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbrplsrv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oerckwkx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ykxlsxwj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mjoynpiq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3crxrsput.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3spfaqjyl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iwbzxfmm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kdybwuhb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qabyxaui.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jyudvmwn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3imkkzuwl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3scdwddzd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wnsupbzx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ncvhzegr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyqvokgp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jeykqdgh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szhsynzu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wrieydbz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gbjceolu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hentviqq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tytefdcx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rsiabrrn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diymumcp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ttoaikhc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gugcrebp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xbsipten.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ymfkieno.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kmupquaq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xufomerj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3csdtoyxz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lqjufajz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxbcxipa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wtvvyisx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjerqkly.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rafzflfi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wymvjuvp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqzkvrff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytsuogum.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3geqdyusy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pibcrdjs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3levcdaab.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hfqfjtsu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3negalwvu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tugwdqey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dcufsqqo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pphnkpnx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqnljpzt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3inygfyjg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zejazbsc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jcwjublf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bksjlasj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bjfuksbg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mncjflru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3izimtmeh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gqomahff.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3prftodtt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zbmblqbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gysqnnha.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iigillvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwpnmbnf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sgmcknhf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tkiconpe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcosuerx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xfotdepl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pktjriuf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odadeikp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fvzhuxka.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jurttcdj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ifcoldln.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3npwecslk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zxrkjpog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3goqdpbvw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpoibfpw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stvamvgn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fuwrgnmt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vlknkrcy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgxcgqkp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgxqdwb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bzewkiue.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rhpsfivr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3svpvwutj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vcrinomx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zrygybag.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvxqiyq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xrzdvrrx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hjxwaadj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wkojoqju.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ootfcexh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3orpjcliu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dixcwbrm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kxrzogpr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tutldcag.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpomrbiq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nliphdvz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmmgiwvk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3emomxywl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3vkabzqlr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jmkamvly.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ecaoniyq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3czqzjwuq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoeahrbp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xsnmhuko.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tlmonafd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3naeoakru.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwtsppbp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ioouovfp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3simcluii.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmxcclqh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rbucoagv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uujejeng.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mnkyborr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qrevirlt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ydzinpxh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vfpofdju.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xmxsilnu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vvepzphw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jjggoqok.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3prwqeqxv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qygscquu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rgdsogkb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vgeahudr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hyfymdsz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gucahxgh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3erujlldl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zhxsdqqz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3taqhprqg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pnytjlng.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmaeucvi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhpofkiy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lpdnffdx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ckunvcvg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pbrjseyz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ixwrgmqs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wzxhgxlo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3icmgcjft.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dyihhykk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dmnmmkat.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wktwudda.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gqejjmjb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mwgabhtb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhavsnbj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mgcqdasc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ahogsynr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rblvfwdk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ydfjiwmn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lpkuurtz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ykcdmqlp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3surrgpjr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lrlkpweu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mopcukga.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rkvadjyf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3woeawxrd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxouchgb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frcaupdv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaitenfj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3imnarxnz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yhlydtna.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cfwbjvpv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywlmhsae.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwcrkfas.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3crfqwbhu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cuofptpa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkfondlm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dyfpjdhh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rlnbiqgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jmbwvwkl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kjqegzdy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gewyzziz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lhlzsncu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uqwytovs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wvotqqcd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zejetsdy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3muspoobz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qxscbmjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nbcrvnwj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mgufolvb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vitwvfsh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rikwwejr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3isgfcwca.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3feugoqkg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rlwujptx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ryekfyxw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoegwqbk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3szvlxitf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3shmymecl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nrzwxjzb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ltmbnrsn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3znqqpcvb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hrpxkldm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nzwtpzct.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ayjuskbx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3evxoknns.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nkqlgkse.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ddayreuf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmnnsryb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qerqoybh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dbfexsgf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uaqcpaoe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmnpxkzy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aexknusi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pzjkwxbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kbliunhz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3crezijws.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nuhtsiuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vohtlrjg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vcgbgnfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmeervbf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mkvfhvql.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3slcerwju.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zoaglrsr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3otaavmdn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ephmoshi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ubxzhcxe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ilrceihc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3crxukoxp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vsczwqad.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ngamtgse.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3krnmibze.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbtovweg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3faaajhja.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjsemir.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3becefhme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hjprneka.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tafgbqhk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyyaqbex.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3diwdyxgf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ogstegmk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ohyxwdtj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lfrbiian.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vgrlionc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rotzfpgt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xstpvaga.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xpmkystb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nkvyzhjq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fcvpiiim.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xftuwywl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfkjvkvc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmxugkfn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3frozgrfp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xqwaazvu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qiegobjm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeebmdoi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cnutnsse.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzjfyfzb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lbskqrtl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kaydipvz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vcffdwss.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tbzyuxfu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lfojothv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nmfmueuu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wcfimxjg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqltpuni.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qonrxrqz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3doairpor.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wefbkwyl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eewfccbi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3epktegjm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fgflrdfv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yoctmrsh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xdndugam.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nwrvxrwb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ngyazvlw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nqnygmbw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3czrvkyvu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hsfehlbf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uikxftvs.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3oeuynpgl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hoyxdgiu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cndmsllj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kauumhfa.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ylqsaecd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nasrlphu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3oppokjyd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3tppgtttg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jsliayxw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cfbvzlao.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xnvttmsj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3aucsfxtg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3htikauwg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hjsojfvh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vdvqtlhs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gizdpxsb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vcockanb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3gtcdbntr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvdostgc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nvjmtrpq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xgocehut.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qqjtfzkz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hzcrumon.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3tzfweeks.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wglvrupk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3puyemjnn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bhuxfhrv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3eqhicxdx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ykqdeyul.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yuxdryou.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kpxrnfot.html


<!-- 参考信息 -->