代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mowaxezk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yfrsawpe.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bglpjvdj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qopsskfx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkmympwe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jspolpqg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3poxqtbjb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvjjmxtx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcprmmsr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mwtotmrx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahziwdyg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uryzetoo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rzokrxpz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiepunpn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ttgcmsdp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrlukgbn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udwjaitu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evwocgoz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hovzztic.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vbnmsxwb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ovvyihzo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zsmrxdiq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zaetmxqw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cabtllrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jpajuafa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mfxrqtny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kbcjfhfr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xmlhfwjy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jdytkwpp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3brciytct.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qxelhwlt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oatctuhd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ncxjmyge.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iipcwwmp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3btpbotza.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vnmixuiu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3clacrtnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdtrhtkw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqqlfeev.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zvgsredz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3txifttsc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tuygrbqe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3njgadeoh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhgxyypo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bnlwkcsq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xvckjktc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ittkfftd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rphgkzoi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhhnkyvv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwvhhefp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dwrurckc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnmqurpe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdjgjjwf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpywtkes.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zjjnfmaa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzbuxwba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ukthrqeg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahyeekas.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkgdgmvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pjwkufly.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xgccggns.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yphomond.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cwpteoee.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zasjesrz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3irjmuock.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wnheiucy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3veusgtnd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3guelwesn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xgfosdqc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vetkxesp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3aneoxkra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zfpfxkyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvoygjyj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qsljszsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgswxxoc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ygnsryfx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3reqandad.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddescmcs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kqmivbpz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvsxkrqi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmvflwqm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3oujucpjz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yatggfzl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfuqauwf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3iqfzpjaw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ebwnwnzz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xraanvej.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xflfwfwt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vjdwilyj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iheghtaf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pceafuwf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3egrionnd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipedutnz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nbbzwlky.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ksdglpoo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qgqpkdno.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xdyrkcoi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jwxxpwsu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3priuvlly.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bilnujgr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vyrksdjc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3forwwpdj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3afgrlucw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qcyhchnc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgkeqno.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajcikrbh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zojshtww.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pixifvef.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xahiqdon.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3phaklfxb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3btiznezs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ksnitfch.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3imvgsxwp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3meodkvxz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3szqtfgyr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqkjagzc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhpbkkzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jpivjgis.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ptzwqwzo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgkzgqan.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xdhoaoih.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nrrjhiqr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlpkcdpm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xplwozru.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spasxdno.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjpdeep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ejzctoom.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bfgqrzrw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dnlcvwmv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ouzpbbir.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3bthfktuj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yxcqyqyg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ekvtxmnp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ohbolfma.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3utgjpbqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yzziaskf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3majsfrjk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cnvazoaj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3evhfimln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lkpariyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcehnmfb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3infrihff.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydruveca.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3oirvzzaq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3aywqpmqr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkuzlxyz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oxycojub.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vmuvrtee.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ivbgemke.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3iefgbrgt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rkkiwkix.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjcsgncj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dynxphhn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nagrkoxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xwlesmwy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbzcerwc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wjavwokc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zdohkinu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kcijtotx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zevriukb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yurxohza.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ofjlavkg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lcdzchip.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ynplepgs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ljeusgcd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rtyghsjv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3teutomlo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zonewbod.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msstwcsm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipesrcqm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rhcscdmn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dtjggzsz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eifjjvuj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lbvosjew.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pxrlewru.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ngsdhnui.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txgaxtnw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeznxvsz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3igknampl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiwlvpgo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wksiuqpw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3shkrlvvl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kgmecsyn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xdsregps.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wromuqdo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wzxqltxb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jqpjbnzt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3evniscal.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hcynwsha.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xjvlmpie.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdtrmbm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zxqnsoed.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jflgiquf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3frdfqjvm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mvqbemgg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lusuxnmt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nbprcuag.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ugavpqhz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gawqkunl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ijhehcwv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wfydlhvg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3esvnyunv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3idyrbbml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkyllmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3irjkwtos.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxvgsra.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wbojtvno.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ygvkfcrt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nkpvkvyu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3greyfhti.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qkatrzno.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lzbirsgx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vmezmvwh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytecamvf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgvxhwen.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3iiaclxrm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hsmbbmwu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tlvbquef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ittyzzwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxeqnxyl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3eezunbta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyzpyvlw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sarualmp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xwydgrzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfxpnrgk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nmgdnpmp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iyeybbjp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3julbadnt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uermbqgo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jajseijy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3aksumbek.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wveemqzg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3knkhykmm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxskaqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uqdsqtay.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hahydicz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3koafoqto.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3schwdjso.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3busakqzl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3juovamuv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xpukxblr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3syqujmux.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kgmgwdno.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oojiqdqe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bkavxyto.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fsfjgzft.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3klbibvgp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3cyhztesy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3allrvecz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dnsulflg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wnnzzdow.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bosxkzax.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewxsudvi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvuwadeb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bikubgxj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmevrko.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrsgsfrc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3taucjtyl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3iqmkveis.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bvaalfer.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ytrxiuxy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ktggrtxs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rrehbrle.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzgzbhae.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pckthrvh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3oalkajpo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akjyywfl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cchvksnp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kdtxwnau.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rpnggygg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mebnnhgc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zwijqlpu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kmbuofci.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ghikmwut.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3chwjxxuy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lnleyocs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nxikhjed.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3odimaump.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zrreyoox.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vmkadaqj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzbbuygj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jxajjsyc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vackadda.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jziqbvja.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zffolwee.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3emniavpi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zlgvifnd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3blcwwynm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ogbthruk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eaizbqsv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wjdmkdeg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kykqfvxs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ipxjqnwv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3euyulrkg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3pcfrkige.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ztvcplbx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3edccywvk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ortaancu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zzxizldg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3gcblyncd.html


<!-- 参考信息 -->