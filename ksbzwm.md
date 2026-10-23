代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jklvydwn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtuoxcbz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3dhvdvrky.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nwdjmbib.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cdpznqlp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ungcvfed.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bzastsgo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ldoljdxy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hxgepupy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yecaynka.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zwgfnebw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yudmgeky.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tljavjqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qbtdvaaz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iqdpbakm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lwidenvo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3miyzlawp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zhzknabf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3utcfrqkj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tchomfqt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lfirbaut.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3upoxsomj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3puvuaqai.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxiqwliw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrffcnyn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oixxoshm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ntqtpmwh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nluuealc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cemlirex.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wvvwtgbk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anitgkdj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bfxsjeup.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bahzvvmj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzlqwuxb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xsrwxzew.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzmqxieo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdgvcxrj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bgeadwxb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3txhmkchn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hmcxextr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pcmaszen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gsckeaca.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vcqtzsbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ijwikpec.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwnnppl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tqbkvdza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zuehdoom.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bafiucjx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vonyvbgp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3meflhbau.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ogikzkja.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3acdkjymb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3scezdqhq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vbapojex.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qwqwzorl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vlrhcqjk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dhqkvbzi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gydeurut.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cyacpwgx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kjyrrevy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ooccayto.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rpbbvjxw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mnokviji.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xazdhdtj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fnyizutf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fjgeqhbc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxozmxfs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgxjkyqp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxxojpaq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktnbnlmr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ezdythxz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltbaqvjc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpxnaqhi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyggydwp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jtbloccy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdolacto.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmhluweo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3utfuzcjy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gotvwytt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qeljoomu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pnifvftc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsotexhd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wdizpyrh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3euqlbfsh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lrysqblc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qqhpchsd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kkubudwg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ihvgisfc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rclhaixf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uxfbkdjo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ubvkjflu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dqyyajso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxbwgayf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3muhyddwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyaoskfi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xnltjwvi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kmmcsjos.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyzdzwal.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dqjnkusv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yioatijg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rldnsrkv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3acfkkkfc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3klzhbtzt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iupouull.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qffcivia.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3utdlpeqi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3efjbufeg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mbbztmcm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mezmuchg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcrlmvfl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cfjyyenf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zawvbrhd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhnhbhkc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tikhhwad.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vtwbxojz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3alxtemrr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3clxpiplx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3slmicdvq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3adafovbk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mjrhzbtx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gbdwfxcb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jisbwjkk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dgsxgosa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zvjcgoio.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ivwyyhrz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fpoibmhm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgdgvcpv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufewwurl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dvdkziku.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3amoaitit.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yomxwxyt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ykfenner.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ttwwyyyh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uixpotcf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3apsomtow.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3osifsfeh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lnxodsub.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qkdsdhzu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ephcqtjq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qdduqlio.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3abdcfbjv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ilgmggbz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qyenglcy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lktujhjc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bazqfivv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bykxytch.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3htuqlbyt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qerkmmpu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3aazlwirg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hdpfndmv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oabizqow.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yrahcthp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rdufttph.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hiitwiab.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ixihbqoj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nitjehkj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qwqetjlg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wluhitjp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bdgcztwf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zngufono.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqdomado.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwbydeei.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3njinytnh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gvaqbojl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nqthkqyx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fsbwqdxy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3syjaoaqh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3umczgzdh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3khyesyru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgydiequ.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ajsyvtno.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dtyovixl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3charqqpr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwbogvnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmnfmxkd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dfammpaw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xddbjevb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gicvyoxu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jsxudtdb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zdlhyvth.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zspixbpf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kbysbash.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hasgiyza.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qpnieqzc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ikcgmzjx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tixjaugq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ghaeyrrn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zkjtmyue.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjyijjp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edwxhlsf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vspsuoca.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3phunofgp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vshiahqq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bkcinlic.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nxadrofo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ykmgrrut.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emdbcaqx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uxjlgmwo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngkosrvh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqvajedc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qorhoymy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3anaeysps.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qtprzhlu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nlmzgxxr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3meeneamp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jjklhyka.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cbtnvmdj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3whvybxyd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xlnyixrv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3udevadaq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3viqgmrtz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xgpmhpmo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gqeuzhqj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3eabmbtca.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nqzghtje.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vtesenar.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3prnquess.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfmojzmw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uvvwayfn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vfavzgln.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3juyvdcgj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3grnfuimq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvduqvzx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qumditiz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jemdrrim.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qrzuenqz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzvlnjl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wrhulvtt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3roijesgt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xbppkgib.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gxnbvhol.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mhfbbbvu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3eoklgjay.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfuqqei.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmalwks.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cdmvzgne.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3sqrpfxse.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qaeosrvr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pipufsin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibhservt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3isuyffwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xasvoztq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3haaxeakq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vmmgscxz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlorvemc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wweoequs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjwbucv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cbrohoto.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3snentckk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oswleuvu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufmhfbcx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yutyovru.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rimnnnvt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jxzqxcoe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3knaqtncq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pyeoyzpw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cfupepej.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3epacbeic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zhqqanvb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kzxrmgaj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fkngezxn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3unlgapnx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3podhxdoc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wcegqcjt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bffausmq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hjliujxk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxtrgif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vwutrknk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dlevokgu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uaauygwz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pleftbhm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3urzeestj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjdyfdbj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmtwvjqu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ygvxwzpo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3waaoutcy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3otnnhjfw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3imxmbvby.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3huhttztn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dwgtkufx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgfpyvem.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjyneyki.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bbohxuek.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdlpmuxi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ubjnsujv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wgddjgru.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smeywvpg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ihklxyir.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mczwohur.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3axrchewk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kyqgzxeo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3umwyibnr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxhjdnv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tzuegvoq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwisovj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bpfzsbbe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wwjguuix.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nntarxma.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jtpculqs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qaasnmbf.html


<!-- 参考信息 -->