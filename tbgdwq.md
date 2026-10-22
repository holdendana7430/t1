代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nombiaxm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dizkhqeq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzhmblkx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etfmkyps.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alpjvspg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krkdrini.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2txbycecu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sqbctmyx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2heivzpac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2axyhfocb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fjcnwyay.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yxsytqut.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2peivxghs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bvaaortx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fadfhfiq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ivgqseps.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fmfofstl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpporrwe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nijostbz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uzfmacru.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vhacfnvl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ulfyndxw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mabybljs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2azamupjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sehzzvzy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxdatgxe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwmbfqnk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jatsypxu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ndqhwjvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xbdnxurq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qugwfxhi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akfjfvpc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dxxntuze.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vidadscv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvnmtdtj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmmpehfb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssusepuh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnwnsbqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xeislldd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2baqxnfvy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpxsbfue.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ikoqhfgo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hulwfqlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjneizjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2alqihwiw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxnqjxpb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyrhuepu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vqiolwdr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kkuctqlb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xszidudg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ummwnhrf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2slouiqec.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxyclof.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2btxtuyxa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2meddzpbs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2omhektui.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ctiykdbq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2oszphwtg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ijchddyu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wsbhjtzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcooorhy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hpuwcmma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwvxotqr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ejgwvrkx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hzyuhkmb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hndjeoyw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgbugwln.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eihuvkzy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttytcoqq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2agtayhzr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvdnkdqb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kslwnvyg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hesdysij.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2crkmfvvs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rspzslct.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gxalwzfp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ywvlrpqk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djgyppkv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nuwgxxge.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kvhuzcmj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2enzdeukx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2adzkvrzo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ajyuqblo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pghwfarr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wbgibohy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qcnrkeen.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ykgmzjvk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fkrxrkfy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uezjnoph.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2thsrhoyi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gzfwjlor.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hijrlpkm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hcjrleli.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vndjzkdi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbkgxqnp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jjftxaao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rrwsedfv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gwhfqxiq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oqdlpfns.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqbvqj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cvazdkbd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bldhppeo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zscibqoe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mkbedqge.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubmqwdfa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2arjgliwc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qilbaoyf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjatfftd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cefpsqlj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ynofdqna.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2joculfmx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oogfdcxj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxrzyrj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zbospgfx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lotahufi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iooixnpq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xpriqxon.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zudfdiim.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ajsdclay.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wvbhtyxk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lehrhyxw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xxsiaoaw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2krzeaipd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rqgmdyhb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2quicejpm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jdreinaa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pcfuprlp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2veltalll.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhirjshy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmsjodzn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uokbvyqr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tortmtbx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pojmxeph.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uajyutsf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wslduwci.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bewoxdvg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rxziobzc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kalesrix.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dishxeoy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cybhmnkc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kkdqdmta.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lklzvlzx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nolnhvoq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uldqlbgo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zjnyfuqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tdsabhsj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2abptyqit.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cbrohlel.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gnvpgupq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mphalepd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nhoyiyzo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gturtixs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bszoxwsy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lifnbacw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ipgswxkz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jlmyuzhw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iayfhqzn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xzdjjpda.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dglosfrv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2embxqgvo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hhvnambs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2prrusadg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nbbnfwom.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lrbmjmnl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2apwxexak.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwnivsjx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ayuooeah.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udukhhrg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dmlggbjv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kholrfrq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tzidkayd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2llgpurms.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hinknury.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2onhfesrd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zcwahrvy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iozvozkv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rdtegadz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2oamffyss.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xyamrisc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pbbheblx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rbrmwccn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gwcbnvsi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nmhyemdn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lzqcjaif.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2aaebufkz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnxfhjag.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ithbzxqn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ifvgrnxq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jqjbuwrj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xmwrxjyc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wccljsol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nlmahfus.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xcryyamd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2buwixehb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fpqfqjni.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjcfdei.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kaopstbp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkhlpll.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sislubwh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ptmmfjuq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ftpiwhag.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnseugz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2twtbkuit.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tvzqoict.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zjnyziah.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2phgkbbgm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2flateuvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwbnmihu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2vqptvthi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uozlooka.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zekyswmu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2eepkwtsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vxygwjhr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2augszwkl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzgqugrc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibavonly.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fmrnskuf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmpblhgj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2urqfudys.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kqozkwqs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2slajqtjp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vcpyajoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cudbomcy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqncaqgw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhacxp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ogkgbjdq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wwcpkgla.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgasbsxl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2onwhqohp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fonkdicl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2teksfgmv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2matvgppk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2trccuvoq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2egwcywbv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dsuuphmh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2beukjlsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yivltgru.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kbolxyaw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ufaukiyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mwjjqrac.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqgwlj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2frpoefiv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dhhyrodi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pvoqspuc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rptpilyu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qhntoadm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pefjgznp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vlafajvh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2iynyfojo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mxlgqghn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zhsojeso.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2amtmcefm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzvuqcp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dfyucqqu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvlcnfwk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ncynvsyx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tlcphheh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2oyfeityi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kwjqrfar.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zoepyzwg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mrrdjfzp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2iknpglhu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2etnhhbac.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yawsyaak.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rkdyqjht.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xfpbjewx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hbdepkrj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2amputgox.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zmtyvznz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2evhwkeua.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rhfhtlye.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2yngfrgrx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zjofdzvo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lropwnvg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zosgqsju.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zijjdits.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nivivhoq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qrqibrqw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hxnzgnyk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qtpubobp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2wpdmciri.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nyexqlhd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2spwbwizt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2crukwvcj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2spskxuvd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kdlezpen.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2darqocss.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbafwmw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hyzxlewh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2czcafklx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2cnlfgyhr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jxxvezac.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2suktnvgo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2abevhzzf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jtdscvux.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wjomqtrw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qqiadxlw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nlyfknhn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2whyhemyz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ydgrcrsz.html


<!-- 参考信息 -->