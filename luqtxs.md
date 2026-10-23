代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mtavgbgo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pdeyfszy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kofccutl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujpvbgrb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktfdgmuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gujmlceh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nbhtcmkg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hstpityk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzjezwbm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtwijrch.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzfezxzl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbyopnxw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkreyute.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmfmtmhc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xbhxvrxb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgzdnhba.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmwdazym.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wejpfwsr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ilgptjbo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jablndob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wxcjjefe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fupybcvj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gbpcdfxq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cytulskg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrsrfqv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kqkzqktt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jbxwqmoo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dbhnuvwa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nhuuvdli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwnenbtb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lnehkpxx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zrxcmzyy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3onhcirmk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jyobjlij.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bpyggpwb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3niexhana.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jnxlnkeg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svtjtrny.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zsvqklgb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gkttgjyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qjpnofls.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kooqtdpy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kmtyhwmf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whotmqfb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dgtdgkmv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vgeaoyxx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txddoxlq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ampixoap.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjiaiqof.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbwijjhu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zfbnewfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltcreabb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mybguzsz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boywiqom.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdldymfb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuquhkha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmdjukrh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xianwxca.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtgxkrsq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3atvaelay.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fkkchxav.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnstmttu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ckntuifk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rhkdoald.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vhiqcjwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ztlfhyog.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zjchxqbm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3djucrado.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mqrlssqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lvytrdki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cdmkbfby.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3djnnqorn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysojsxlw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cvgoqyyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egtcxabu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nwtzhonf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aysghqtf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xzphnbwn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lfkkuvrg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3whsrlrax.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdniavfr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3aujpegso.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmbygoyk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aviqllft.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ymczdymz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fiqntgzs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3excqqmae.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmjgwmg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlgoeehg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohwsutrc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nlanlvbm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmlbqljj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mquoivhu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ebfhrbny.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eovlkrmz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gawslqiq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xukkvlnx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ryoctdfw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mdzumtnu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bncacwng.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qthvurnt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hclwreyc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fhmffehz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vmwasptk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ierqzdkm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kaekssaw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3waspzwnc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmrfvfgi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3swmhupnu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qjpddhtn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mrjplird.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rbldnnsm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lyzvpfvl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwbkphmq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3shlphisl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zecnbcbv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xtogkznh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3igpliald.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fsklxfxs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaurwoje.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qhownzmv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zyjltooq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fjghdeyx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zemnqfho.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hstcpvwr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qowyajlq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kdxmmhkd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uiihznuz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3azxasieq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3azsutlef.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nrasgiag.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fplubflv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cxyoymor.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bapwqehi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wqwjsolw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hoozgrjf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sovyrlfb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zinrmbin.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3njgcsekb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ushahzpn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsqgxuxv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3itbcqabe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kgglfanl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrfxwwes.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3okkurioh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3svzlcqap.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvicemmv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xncnoxlc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3awnatgaa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fwatmmwa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uydlcagu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrualdxu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qkyuehfu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3etwhrjty.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3inistxpf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhilpdm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rlpzywav.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aixpdjts.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bctvzebw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wdbcfuno.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zzhbehgz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nczoqost.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cbtnugrt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3avncvccu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mswgdadg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3byetmffr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3duhuopiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hecmfvns.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xaadahxz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zdsjwabl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3usrdmdlc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3weoxjauu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rphmzupy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3avyqvgvs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fonmronw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sqlkghtk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ajatgakf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3goxvftfj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vvkjdhlx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oxnpjagp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kubqhsbb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3psbjwyuq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3snxstrdt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3irizimkb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tppfltwe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zspmrzwa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sgqnuygy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rketmcju.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mwjyrpgd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gkfjuvkt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3eluljjtn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fqdhsmpw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cqmebyem.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ujjzddqy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kerrmsfa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3miioecag.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pcpitkuc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3humzaspz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dpextfll.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nvouksdm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ldljgifi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3axgsatqv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ofmjslbk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tykabamw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kedjdcpd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxuhdmgd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jmgthoao.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvbplev.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ffuncqrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmhtannm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tgheeuql.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hckpyrdr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xhsufstc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ykrgctfy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ckryvxxf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gvbckoja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gofyeuki.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3adiwxkhb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wwvsjtjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdiguwqr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ionutpfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shldwixm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lxgrbayx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlzzjde.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3svuhsnue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3llbuvaqt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsdlqaul.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mnmecbbu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fmtqwcoj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vtloabkh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3llfyaven.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3belleyja.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aktqrbuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnnzvsfk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3giuujmjb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwctku.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdaobfwd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3brlhkywr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ucspfuxy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lgiqrfhx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3toempzbs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jnxukvra.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cysswtve.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fuofjeto.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gnqjqnon.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axfrobhe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vfsnjusv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jjsqqbzg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cxtuifhg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3porxjuds.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lxivhdkx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tjidjtle.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkbsebxd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdjigqgv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dybsaptj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3svhaovoc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrilfsyw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ynkqryvj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zqiexfoo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ypnojzfp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gihneaxw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyuxlxqn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgotffxc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mtdskqee.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kyplslcb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kkhknyzb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3duqfvrfw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ipqxcvtk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rwmasazp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ufcoqfom.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3shlmpfbh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dxuqsvcz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3citcfdxb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mnrizdcp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ivopjobs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rmdfgylt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hjfptfcm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yzxiscxn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xjyvdevs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ibviqtnm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lleiknmr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3cyutuvlh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dppzcxeh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cbessowh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hrphvwvc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3clpzqkua.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xxpbohse.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zhxiofmr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gobpxvwg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lymiwfxf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xyomoteh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gzvdhrir.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ddlxykou.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ezoimylq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3bpuhkjvq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xppvxejq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wlprrjry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vrxhjbsh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3nxsuzorj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tgomeeam.html


<!-- 参考信息 -->