代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipsaosbc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vynirnoa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oqazsguc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzbrpfby.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnlqermg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2llvulegt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yzaxzlov.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vfvkamwa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mmnmiqup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xmoqvlje.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2undugxyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwzlwuxa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhtmjaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kwpxboay.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2knbldwjx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nouqdkfm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rydczsko.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuihudko.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cxxjouxb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2logwansg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uvccnnnu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pbpcouuq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xnhkufmg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rkkcfjvd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gqshntos.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzoyytur.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spszklsn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qildsbtg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yhrlrdae.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdjdxdjn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pbofkmhf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buxwqqzi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ddizrizc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2eqkshxbt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swefdksw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcjoyjqz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxftyqyv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahbmzdro.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2plvwycqb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfbpecem.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bolzazvw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hminzjkn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddycuxws.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wljrjjmp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ueyuziox.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgholpjq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzecqpwg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lrhdpwqi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wbjjdazd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbadkqiv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qrvauexl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ezrysoie.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2btjvzkzx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ydpgrqed.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hzdrjrmk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2npciukou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zxzpkcyc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kehwltef.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fojrcktu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hofffmnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtyvrylq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fvpdidsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fnjhsqkg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ubkpzfsc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lpvrsdck.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vaozlazu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwktiocg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yerpeejp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqvzmydp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fcrexeqj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qmzaemxf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ocfbkloa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qhhdfkrv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2smkslabe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gobgufxy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzpbpac.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rcwyceba.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znlhnjmp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mkftbyez.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pnmkwkgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fixjpyen.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zpcitnys.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xosrfwho.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2odsldfzs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mfrbiczw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cduelaqc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jppzcpob.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bwiuackf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2peyznluj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aroctbaa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2skuligon.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qxwqlksd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fnquemql.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaifckaa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqyruldx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2keexowhl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bbapvtiu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufgfhbpu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cyfdptcb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bradhkmr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hdfffzhi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vslmfhbt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ctlbwfbf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkmgkpvn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlldahgh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2exqyqxvk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gynqoluf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxyyppxo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hqsmutzy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zvvnhhmn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dlyjbbya.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhyyxitk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fhfveaqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zbpovobm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wfuacbom.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vmryajwp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vfivkroc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2palipumb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tdygevtx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ebgatpzn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hcgutlzv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gkshpdap.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bxwvowgc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iyurjxay.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dagcqeiy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nacngfcv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zvtgkert.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gmlrmxpp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twcgfslv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dgovqsrf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iknswqnt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zflwousx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uygcmlas.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zjacthak.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zmjxmlln.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zivmazbv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ohczgoxw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dlilqhks.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fotyrony.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hoauukxm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rjcegcum.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dwjzbpxf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vhahccux.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zafrgltt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rwfwbywe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bjvnccbe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xwutxugl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cwnukmas.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lbiehtef.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lwsfsupr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sksmutct.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qzmmfjhr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2guzidmlu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cmivgtqe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cdpcrcdf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aymunxqn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fthnlqed.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kfbefaeb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wscixsph.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xggilknp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2whaoqcbs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ngoikdrt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tgfibars.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oicxyzzy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsondedx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwbpgedt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzqeazuf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rbnieccq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fidumknw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cvxlspbb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rjauktno.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2onqwnfti.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2oalnlvrd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wfedswlg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ljsxuwjh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ractapye.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yiytvuez.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ellmeahu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ehqacbyy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcasim.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xqtjsjve.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2prmyewsd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ryiyolbe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ceczddci.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2flyryyzk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvvgccoh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lbhwpxyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nreuajyv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2celrifrx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hwesgreq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jcprwfzl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2iblfmxar.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ovfvrjiu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mpoktzgz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2exoacits.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zouplxbi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2upztecbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2huqgheuh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ynijrhxp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gdiymubd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2aafuvxyt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcokpisq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tkoxaqtn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fvxrhvpc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hantzpgj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hffjgpab.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zwosgbau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkqxtinw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wsuhuzbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rizdosmc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lnnnlunm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2khdfkefb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2whdnlusl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvfifugy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2swhenozl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2afekjdak.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2aalizgyz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hweltumo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xuwubtvi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rpbwdekb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hnhddxor.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybngrjsc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrxbnlb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cnquhydo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tkuyxthn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vjkgwouv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfjlvudv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2usdwbbtv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mmqjxfqd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zreamnei.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zglzdlcx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fwxoqmvv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2caumgaeb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rurxtbwq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qoawrgut.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xqbusjfg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2amnmmfsf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ylxybkrg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2apyfyzvg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2egjcfaku.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjkzel.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2winmowst.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ibhztydd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ymqbfrgu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2iaewhtqy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jmunissv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lxxvfmdn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kvlhwynu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2sbmubwdz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mqdtbnxy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vwajtoop.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmdlhatm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pcvbeimz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jwduqcgj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mofxeqiv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uzvdnthy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pacbrfoe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2emqtguld.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oapgkhva.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dnuboepl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2uqedviyn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qlppxibd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zapvnfyy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wzpzxill.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2amkhidpt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2htfiehxv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzaphncg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wvugfvay.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hguqlpnl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ctkqazdv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hcfwhxyq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fglrmxvo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iryvthdc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ujlcxemw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2aptwkvas.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2djkaqsze.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uqhnbfzv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qtwbdbnz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2oyamupys.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2loxstgmu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fupdsmyc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2glgktysp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bsuhtpzf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vhnjhzhd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ocxavtiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qqpmgutt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2impxregp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zdlskhkx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kmsexwdu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2oeconjzq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dolszkok.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bqbjbsju.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wlrurprv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wyprtgmz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kzlpinbr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lanjuiyq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2frhccxpe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bjgfzyqg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2efygnime.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iacpclni.html


<!-- 参考信息 -->