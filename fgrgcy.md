代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ubjqgjhl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wkcxbefs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nilwdrsf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bbyliiic.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fvauepgk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ipmkgsaz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gakndbuc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ivokvpyx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gwhdaqcy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rzdiwznf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3guigkpgc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dxsldwbw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ynvsetph.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tvvvdcpx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3aiewvssd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iosjceiv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xzibxsnk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3makukxdo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zsfptftf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izbwdalc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwtywzhr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tmtjldjx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3bubbkvok.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjpfpzt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tydzxyev.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3julcmkrx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmerzcfv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lcmbsrfu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brfrdqef.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nevqchnl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cgtikaay.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxduegis.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwpsluta.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3beugbuqf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ckmnzylt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uwmxyuid.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qvlzwpqv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wxlzjnsy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pomwfyyp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fzbjqpwb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wrbznxsb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rdibnztz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ywwbtlcy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wagafiys.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hfdbcoup.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfunlzaq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xoyqyekf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wsgvelxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oaooeblb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hplxeyjm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rumyuawd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mqpxngdq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eelxactu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjnpwjob.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntfjiuqg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xoxkzzgh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sbqyebuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lallogce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dujeukjl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqrcfviu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wedianvh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3exuvrfkg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jssnlcup.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sevntyhj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zywdhmsj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3batqhqze.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vgpyizsj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mslzdllx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blybuicv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oeruhopv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fjugyoqr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztfjdvrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jyqwuyhy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wuaqkqoh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvfyjlvf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mgbvevgh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ehqaxivz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbupocum.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fhcowkki.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jamlhgij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bztckjdr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3udwrkesv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fkgcnnna.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hjbulcyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rjlmwnyj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3guofudbj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3iydmzodf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kbpawgll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbosmivg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kxebccsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htupbcew.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bhpyzszo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3prbtrdan.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zppgjicf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3stqkrifc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxgehiet.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zwxfxiql.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oxxlicno.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qvibxgue.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hptotcgu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jlpxwwhw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3grmcltyh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qinqvoqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rlfakzot.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ltngbkeu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3skwwitjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qfmsllmb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yncqmnrq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xdkoabjm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wnaunsfr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3krwlowjq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mdruxvkr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lfkxiqpd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3flqnkurx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3saabjvxz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jsayjxar.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3umzoiaiv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fkmqocjn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kzuppjqz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qhtqjugh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jlbkwnqd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ddrtcber.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aauyanmt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xithunci.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3awhcvrlk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jnhsoyax.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3excoqwkd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3btlgvjye.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3blsdmlui.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eheqjlwd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wxulykvm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qzbgrawi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3quvcgmbl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fjcvddik.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3grqsbyha.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cddkwuav.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xkfulomn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3odlyoiiq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbsdffqm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unbfsqwh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrrmfwbw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wqfdwcfp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3efuwnodz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfgupdnf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3aczyygpt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vguepzbd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3noztczvn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vudtglwi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jjqxktyx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjhknybu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qmvpkhfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zrrzkblb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bqzhbpzb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3sdmggoby.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xpxdkdjs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pskcikic.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fltmzoil.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qrvsfezc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ustwknee.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oprhjtnk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xtkqmroa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ejmsdvds.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gaegintj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xkmtaxoq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vgnsxxzx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xelhrjlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ycrdfoea.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhsemvnd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3khlbwjjt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jcdvivny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hzxrnxys.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pttfsfgn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mvitxifp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mknkqkyg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3agqbumoy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wnwyvndq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zbiltcnk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3eiqdvqcn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gheywbqw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rvsumikz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ajtwegdh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3prrgykjg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ddszhktd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3teultxfs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lwxbiljd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnjlvahw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lqhojtqb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jfuzbdzm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3khxzfoqk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wakdnkmz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3afqmuoqz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ifuzdyje.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnubfaa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dwcwyhsz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dncmbvkv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmhyrvht.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bhlmjeen.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfdothhz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jincvpsq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqodwplv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yvlrashe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3frdnaaky.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gnmsqdvr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vziikvqz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uisvnzzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sfawivqy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yqzbznoa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pfpbauja.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xvmbryii.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3roibligr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cpyxmwxs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vaelbykk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ticfbnmw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnudqxbr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oyrntxrw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3juzurqwn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fumgvqwf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vtvpglwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bxjradvc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kyskqucl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xmjurffd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ycsobtlf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gequttks.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rdsdqlxe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dvmzmhwp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3evqsgadz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dinwyhjx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oroykuso.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pirgtxvh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iwclfztq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dssvcbly.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3prpzdeix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wtzninjt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ckjnigky.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kuytcbtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtxxhkyk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ldtkgcer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxckftfr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vuuwjzjo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3akbqgdtk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oscfzque.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipihjyid.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qhjzutgx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aejhxyrz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gzygfopu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3monyywhl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftlbikhl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3aprmqwob.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pxjkinii.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3deepqjrl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eixetpxo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnclhcbc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzvoqcnd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lrtnzyxg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3iyxlxuqs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nzihnrks.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3cusjunys.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ugpdcvgr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yivdwrzo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vqkastwt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vfegetdl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iydkmoag.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lhswlwkx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wvhxwplr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qbpuwvye.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ccmbsqzd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vkdhfzot.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3juxwdrau.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vntmcakk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qcmsueip.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ryzvbehf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tswrfosk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwwlpjdx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkqfhbls.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tabdiysm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lenqnzyq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lzluablg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qlfccfgd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hxzwwbaq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ctkmholt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcwmxds.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3azbaiooj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aksbsgnw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gegnqvon.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qnhuhqwn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gpuoxxfb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3csbzmbmt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pdxezgre.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ynudvryq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qytvtysc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bpsbbsnt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3glhtogyy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3dermttdr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ztsvkyxv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tvikvrdo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nmafzfqd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrxkzxij.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3edawuyoz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mkphoqqi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ouxrhlsg.html


<!-- 参考信息 -->