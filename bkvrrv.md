代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nftyslzx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bhqkgdzh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oatcmzoc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ysweaswc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkiljjiz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tawrridw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yzpkuimo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbrfgqli.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flqehxmq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2srtqanfq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jfaqdxtc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wrpusmqb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2illziwnx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vsxjifwp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jfhrvngq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xzsgbxkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ysnyzrhr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2riuzmkze.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fiiaybjs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kxlpjcyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2aildsabz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bonptlje.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fknhdpcq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2blnyletq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtdjsci.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vbtlkttj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tspeioxe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2filwlqse.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cbjmoyug.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxrkfvjj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zujpvzvi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kyywibck.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qixylomn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ypsvznkt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rfmcdafy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfvosael.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zvdqizcv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ewemgqus.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltmytjzx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xsscccbs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2csfeqwuw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjmajprk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2oupwoepw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqfcrfpv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggxqchqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwocnfuk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pcmlhvhg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkqgmvlp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tcliuwci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnomehsx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frqwpscm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mxvxldoj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2houcxucy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygzerqak.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ycfitrku.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2efusazzp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ebeilesv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2daetavfo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nwdggcca.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qadlqvlm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fabnxoar.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gyngtath.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oleqcijw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rdxehzea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jruaserr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mnzixpdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvxohwoz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nxsfxbee.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fmrzpexz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmtnerps.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2abqrubjp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjikpaxf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tttmzupr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yizohxkd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xezslefw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsyhkmeo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnjeposs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2unvjudyh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pevofkrv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fsfjekzv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hdbyanio.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfoalyky.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2icxmjnbe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zftbsetv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eczsivft.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jkjjfvkn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xiksinoz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qkmbpyux.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jhmipdhn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2edfoedlp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qapcpodg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2koexrfly.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zhbgydpg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hroydzzp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ywawnkyb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nbqaddjf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eajbghst.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxuibhrg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phqxeswn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjoaqbvk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yauldthk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbftctqt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lovawsoa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2oqtvqwct.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cylqjgjj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shxzespz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjhocrxf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwkhwhdd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmegrnex.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2skrnkoog.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fhhsudmj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yipkpyxe.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2isfozyks.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2csvmmonz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pxnvtosf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmeqlzy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hurohsvu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2anufnmqr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yujeuwua.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fqtrjoek.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lcixzrdr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kmgmyavi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2izfttxhg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nkuvomxs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jknrhqyj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2inugtybu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2klhxqlgp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nmsrqffp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kcbmygyr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zaviezbp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2oozztmyf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2iijfcmco.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2opxukfuo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nffjehhs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxtlrcdu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hjptkntt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mfxtlpge.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ytyqluth.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2folpwwlu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yryarupl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xxouazoe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pkfxzebz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zqgeqljd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeoadozj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydletgla.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tffziyrw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qtzvgpte.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2svfqaizk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dqxkncuk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bymooext.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kanoiurg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wakoplvw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hztjyvuu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2elcaqwda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qouflnpl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mlqtqicd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vhtbyssp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xwumymer.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mjkipbks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oaplomjg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fepxajnw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2azhdiopd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqyrpspj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tpoobrbe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mhzcnbbx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2thnnisvt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuzjhyov.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ldrfncow.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhyopeeu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwzisnzv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wjmwhneu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jmrhsjlb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2icpoobmm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hadyoswt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ozlygdpk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2psnphoze.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqijpns.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zyvtinhp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fcqsxoxc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2czykljqc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sdqcfcke.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tyjggquo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2psikobvd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lslghvng.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2splysndq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ginhdfkp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kbglixfp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2prbbawaz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2itcknoep.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gmmzmapx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ojxcrnpk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xpblnlcf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2uarenskf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dsvktlth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pevlwdzf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfqkmipx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jsmgzcru.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lwahfyxa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gdcmunkw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2klyazgnn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gwmrhnbu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbxhdfv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wqyblbgv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ppzlshaw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vudumuyd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wpzcmrlh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ksajepmd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gnkftjuq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wqwtqpop.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2auwptaio.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pvawovqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdwaagvw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2igtxwvqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzwjpzxa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yeulzbxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hcdpqwyu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iwvqqsuj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2muiqjyfl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2okfmdtrj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2auamxopu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dvkpvtgx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mpgrclso.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2plzphrev.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qwiwmykh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ikfarkyd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uqhberes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vgtnmnmr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usggitdz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plxhfoob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2niynryyc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2quxvoeek.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwklkrss.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ydbscnjo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2cytysajw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2swyqovjt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yscxbbit.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ytzoggwi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ettgvrtr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2imouvgcw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2clgyjuyb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ssbfsmiq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wzfclrxz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rlyuxlbz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqkmgdku.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kavyvvmv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrxxprik.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhstngyy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2uamfmfpi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nrgdumib.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xkflutvv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cfrhapzr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2sahjbdtr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ubmvsuad.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmgodqzx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vytutghg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vrpsmegh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nqqndyms.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ikswyhcs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xntdglbf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hfmfwund.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jfcibkiv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2johovnyc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xqliqnhd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tfafgcni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2erbunjqu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fpjrtxvb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2upngwcly.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tcqnokwv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zfjhxgve.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kwbiycit.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tqukjxvd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ytzcqusc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sdzusqve.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yyvxeyfp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wizanwcd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jgrlmoue.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2boadlirj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nztpwpma.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kdjkyxkj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dwcvinuh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2iigbcbpg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pdsdmhkr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tgedqrzz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uvgcmuca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2whvdfvzo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rzdkrqav.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2edvavpdm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ukqecbud.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2aagnqosb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ibvzhsdg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqldjsg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdaythnh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2uwsjuato.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wtofzpbm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ojguyids.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fdelmpuq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2zuxmtqnn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dagoyotm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zglwdzno.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eorufpaj.html


<!-- 参考信息 -->