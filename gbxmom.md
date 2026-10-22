代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrhilno.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2suwhlyec.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klucxinw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rlwhvbie.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhylmtrm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmszppsk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zfvoycst.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnzralcf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2onpxkzip.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agnhsgip.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2grqkcaki.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dncxuswz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eoaxwfkn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ytjxsgsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kvcletmb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fikuvsop.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pcampijq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ewapvugy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2awxtxmlz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bqahoedh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogytijlj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eksalasj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nrpmvagh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nesftbxu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yhwpvrdy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dbmipyar.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mmehplsw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zcyyoykl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qeakvtvt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svlazbxa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rwbjivyy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xtbrofoq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xnsvzdxk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fspmavuf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qlhslvmj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsgbuffp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ubvdgfcg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tgkyrahp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfrbaqwk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lygairyy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqeqzjhl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvtwaozw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ldddzobt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjprloqj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtcalwgc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfejsejb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wdunwxoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mphpzvrq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qblufmnv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gritxqbx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmknuyut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmgcpl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qsffugur.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpzywymh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tnjzflhb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sltlksmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2beyaqmug.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dnzrdalq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ojwoufwb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nehxjjrx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dpcnbomq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gxslvysu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wvicuekv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ntxjrfue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2msifiigx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gfsnksel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ochzlijk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2seioesjf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2axcycsvu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ujxysumb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yrkexddj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kckqvvqp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utrkexmn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sjdvswna.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2itxxyary.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtjygqrn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xivqpwfg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mzawyekc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbaifb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcajpuhk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjzelfaa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpokbvxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uwjyvdjc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2crynudhc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbkqvrow.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2emryafzb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mvspygfi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ytuufkwk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rzwggzpq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ygijpfes.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rjqhiohp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fdmyrmsc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gioxngit.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iqmruvkn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tuyprcou.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yrttwmbq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qajmtybe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amdgbsym.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kehxaaqa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjivtol.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2krlavhgw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zqbwqasq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kmenlaqt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ybcszwfo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tiojqxvw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymqzuhyw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjbekduy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2viiorsip.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rxpajupk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ylklmkcc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sszkuyvr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkyikjxi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zujrtndb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rbfekjeb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szwqglis.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rauxdrvp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhmlyklz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbatiia.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qvqqmqwx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jxdcpvvz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vcfkldvu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uycmqdmn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lgooqblb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mfwmnvwq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ifyawarm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rjjnzaed.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lcqnmnnt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pnumxkbo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gexecmoo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fonbsltk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sjrwbgwd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hroccwxs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yokmjkwo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jwuxekhd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkhpocxf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kkqotuew.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2sbxanqdy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncusadow.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofxrpijm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2epfbjqez.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rmsxvulc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hurnuhaj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iwnoqzhu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2affvqeki.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xdxmjqdf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2olhoknnt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ipmyfgyy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uehrfpxp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2aajfpumr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pjxtxpau.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qpgagpxf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kgbqfbzo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ynejqaze.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dqkenczt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wbwovifp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pegprhxp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fdcbchyu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jgudfayj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2axlfmwqk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qjlaeybs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2snnquxvy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otmefqik.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xzejunqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qvyupvyy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hcdzwlwm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2satvnubp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dodjeaxs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uktfjtjj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yliargjs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wimpvwuv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvktiwko.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rvpcfldf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ootzrsrk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uuyhalpn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qgrgjvvg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hisrmcgs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zxvptuky.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lkpjliwh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ltfxhyfv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2shdbllah.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kqraemca.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vrzvjiaq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ilrtfond.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nurntqqz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vmtdkoxe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cbhteewn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2amnhvuog.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2thletlon.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2swhbhkcy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ghrleeav.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ywallyix.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pgzhmcyz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ezuxosmi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btxvxztk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fqtrtxnu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nayevcgr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dvtplozz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxvenxmt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2drjjuwgp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ieyzueny.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fublommp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytutiiyi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jbkmehzv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qsfguqnp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wodvbpmw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsmvwikd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jtijeazb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2svtmtsap.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qvrmmpwl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lfexeabm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cwmuglng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggvfaqpe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bjxjhsyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxsuscae.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wjryyoga.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bymiaztt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwwulfrr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jkzigiyg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ugnmhgsx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnjanrj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gdmaihin.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jicyojgj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yfqdevmh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vdunhmbs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jedacfbx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oifimhxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2owhdcabu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdfzbocs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjttyjp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tctryduc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yuybmxhq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ugaoxfzg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wdikdxbv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2maqkpljq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2clppnolt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2myhonita.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xcamfcry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rfykzfcy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2guyseccr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qlnkenij.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xbmairiy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fjdmtyfg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zrbmymkp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmhxrsdr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gwnamydi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mqjgfrco.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aleerlpi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aehyefue.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2opzfjyht.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2arqbuhyl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hjtagmls.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wqynmhhf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2goqoixqt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppipzpvs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ibujggtl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pxvzvqqu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ueewfqom.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tvgaribh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kjhfdrlx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xsqbvawz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fzthxsec.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jgbdggiq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xrsdbdzz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ocammmrd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2omuaefgv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ehjnwdej.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fmsasmhl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2asnslquo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ykkyxfab.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uwayvkkm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iqhrbrfa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2megoebxe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wqaewrxj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cqcsaael.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zzdqoofa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vnmmdlqu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dqfemejw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gnhpqtuj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jhlkgnix.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2plnptchu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dvlkwygk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbkslis.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wrwohlsi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lfnttwgh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yalkwsmn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2rgrqmrqr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cxpskmoe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pbdtfeto.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2scmuvxhp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qitehmvc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2znuoiqsi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2svlvmbaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kxxuedmh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2drogtbkl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bmztvcbv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2meqluuyc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ahsdatgd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rdsbypdm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bhzdmuns.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rpgraigt.html


<!-- 参考信息 -->