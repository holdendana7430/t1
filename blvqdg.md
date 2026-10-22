代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2oaxedowy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2erzebtdd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgqkgvom.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fustugrn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojyqobzw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmxnqzvv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2miqlxdsa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfsxcwxr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjkmoifv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2agdxsyth.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhlbfuxi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkzlfayj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klnmjthl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuwfieus.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ruugwvhd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgwfkrfn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yghajynj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrzmjkpu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2sbmlgcup.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2shuvtbkp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hrtuygjl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dqzjjiqi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uqvjoddh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xtxajfwk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hatulcch.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrypfoq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2laftvawh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dbioxjwl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bzvfagvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2khyagwor.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhkeqqo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yiphrfak.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2euonrkxp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hvfivdxy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2okbklazx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2diddzarz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ynnvhokv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmzfzoyh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hihfmoon.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2frggflln.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sgmzlvgs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ehdbovst.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rdqgxlxi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrkpfrjp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kkznfqfg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nkdfgyvh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghxexqna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqzordtj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdaarliq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddivzuae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vyctzufl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sykfbyvm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdvkckqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywuyxqei.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kvirbemd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzyuvtoj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yryubfcs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byqcvatl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymgxhuko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kxznihrk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jufagdtg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftfaslov.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ukecjfzo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nljkxiub.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xgdxbgvt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pgpufnna.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oeqyvzhi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ajplhaor.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yrkrwjdm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2irdqksoa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pnfuwkow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kphetllh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtaucyjm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zzyhldnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oazpppjo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bxzrnqkw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xljlguzu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2whdjqkek.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqtjarjn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlfzlyj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yofpyhjp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2golymsap.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxqwrytf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wnllyflp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iugmvsou.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2airqoazk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2opolmghp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxkbeqa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2feaoicfr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ordiomzb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kuysmppg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2evswjvap.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yasadxja.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zhegbvzh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lmpvjnce.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xokrrtwv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tsobtnvi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qnxfizzf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dggbgdqm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zdqxwocz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2htqdfawz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vazzwowc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yjinorts.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cqruljry.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qjlhport.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqveigob.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbkqfoh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2icjdkupe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tfrkocmd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mycxxeiz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wczarvfy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jfpvvmig.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wdvatzdq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lsnacjlo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rikbwryo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2svcfvqte.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yfxpasdy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2brifveil.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2knwttjmu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yviysnar.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ueloidas.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nkiafolo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qjffbcas.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xjderbvo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxjdchpq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ltsbunpn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2iscdqdto.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuqeyvtg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gjyjuims.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2snledkwq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wofzpsfl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2scczakpp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2juqrnzye.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ymzpzlwp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hnthsjtd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vaufokpv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wpqjilql.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rvjxfrfp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ltdrgwjj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wdxnxmet.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuceriio.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wvfxxpou.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rdslvjhf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xajiujkn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gdykpqjx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2eygsoetp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpytxyum.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rjmmdjtx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hgyovsdl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mhkpsdsv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mjdjqteh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueyrhpru.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ixqkczqe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hncpxcxx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zmptjual.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yzdhhput.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lkpcqgek.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fjcgfcul.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xvowbsxl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2diatncnn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vvjxfkkn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2efzwroqf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nncwyzeg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pxzjjjbb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oecvgjfm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rjfapmtp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dzourplm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kqpeeecm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tehileka.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hkhmavtc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2laxrzfop.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xoupgdzs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hdsqufyn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgwjlsuf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jnwhtgea.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mcxvnjlz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kjlohhow.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2blgslqlt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtqlzbzc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2caroeslz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nedpymeg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oijvljbw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ksbnkrke.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ldubkdpp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbuwjsw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pspgudcx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cvyxbyep.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hlkmttdm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kjxqyfsp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ksvusejw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2slyjvykg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ijtksfwi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2sqezwxlc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rwerdwcr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2klatjedb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bxgfewmp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2acjvhbvc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2inwacmtw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2crtltowx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mytlxipf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zzxoflta.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zwjppkwt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yumpqmjb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qlztnrmm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qowiqomo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztkjmrvu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bfsixhtz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bfywkulp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zjqfdhfb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cmgfwtdg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mstumaqs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mchflckl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zquhwrnb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ehicblkp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkodzrt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dacvplig.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nmgueswh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2byvqzqgl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dtpdclll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tamahykv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mmphqbiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwztalds.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2omanorej.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fpufypnq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyqbvib.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fpdzpdtm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ggkovhqm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gxlejkqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ibiwvhsz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqrqanaj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2itfkvzpx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mwruazhd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cbochvci.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnonuyvg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ufdazehc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojpfvhuj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pxmcttdq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2clzteibg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhuyrizs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdjvsjlg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xkfpnnjj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mrjfaozh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abjjvipz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fcmtedcd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bhsvaemz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pjpdzjga.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2txaqfege.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2uzeaqijb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qnkqncve.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggkrpnlr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zydyusct.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyzxifro.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tdsrcgvi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vekudvdh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvbqoyei.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vcppmxyh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tmdrehef.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqdhmqbx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2npadjpoq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2huxrvmzy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2egasensb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohdckzhl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzeeefsr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zxwfgrzt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2yvoamehv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pepknixw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nzxfuaub.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jlxxhxlr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2viaskkkq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ewojbbyq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2colupkaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rozzawpg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mrbxvoqo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ctjwzwjo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qpxrropn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dwbkgdgz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2htfibygi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ybhcpnzj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mlnxkbqq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rxevoiri.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2apgjwqdw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wdbkxxvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nabisqjo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pusolomm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ttrwaazl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2acyplxqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lxvdopoc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uczxxogo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jeufyejh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ggjipyjj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hlhpedrl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cewapaxi.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pxnvhaaq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nwpxhpyh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kbfccbag.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pfhugats.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rpyuipmp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2msizpryp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sefbthsm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2teqpckyg.html


<!-- 参考信息 -->