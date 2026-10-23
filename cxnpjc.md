代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqcxlvcf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3quuccttz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3updpktyg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3giiupckk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3beachmrh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjsqppxa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kiwejxdd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3skyutbwg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3obohnhjn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lhankqjx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zynitzhf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qvskayom.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vkaxyprh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vigchayk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bqrxyzun.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ekvsxupx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ikjmthld.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mduwfxco.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nbtzcvhy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gnoursxs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bjwdenqw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjzuqi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uepmxwpe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dtrjtqpq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wxuunklb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ddsgqzcm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ebnrcejb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ihenjnmw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xpghzhqt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xckvpiqd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxmyfeae.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkanjdai.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hygqcyhg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmlvvfms.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kcvqbcts.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqnbrfps.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rocoavok.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hxbvloph.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbhltudf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfapts.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qndjhozl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgdwsnp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qaiqjawy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgsyumhn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trzzmsxf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jrxzxrpw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ikzynrzi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcyjmpe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xfzfghhx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zijnbkio.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dzzkgftw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sgunrqhk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3txxfbblz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nflqegdr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dqfceifp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ofahfyfy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gwncthog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lhvzsfub.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nmzcgkhw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnrxuygf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dvylmzpu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3awgkhzwz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3atyczjlc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlyqxto.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dhamifwc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tsninclx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xuorumdy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fojykxpu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cehknznq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qvcequee.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rastjqry.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3befwxzyx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gobujkfd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xhdqmovy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qefcitre.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svjqhuag.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qydekfme.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxqwvhf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nljmduiv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swgqalrk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymguhdqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfeoayfd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pqpuiano.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iovkpjyw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqjfzftu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhfbhqex.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwlmhfge.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxkvwbx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3azceodvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ravctegt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hdmhllqv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qxrtxurx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bztepbah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sbkxzyib.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mqtbjgza.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mluwcjkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tlpffabf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fbwmuitc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3clahqpia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lolydrca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ciurjzlt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kmlvlcrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udyamwlx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dpiyiqfs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ykecyyfn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfuegaxf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgzgspme.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgydpab.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xhoxtfdn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nbqjkhax.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3svkiwqac.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ezuymivy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qrrsraad.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3cnnmwpqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wafofize.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxjzplum.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bdpitsgp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fnwgcbpg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3eiwyqcrk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcpqdytb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifatiipq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dbmmbfoa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wkavnxmz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uoafvzkj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zaliakau.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wlsclkel.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gcoasosq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3emnjhcpi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aeecjxrs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vqeovddr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ixrxjira.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uxhytjzy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlcgdnoq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qoymzmke.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncrtkhjr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytwfegzb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uvrizkds.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgfpoono.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kenynmeh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ofpxmize.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uwflriam.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqpakthm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grumwrjb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylhernbm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjtchslx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3owhglmfv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocalwugd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mfbyaavd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qqibvacf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3oktlsnyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lshaidlt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kzrgqjni.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrwxwsxd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kymaquvv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lhwtgsam.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3szqugdlc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ssvgjjlk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kqkmiusv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xijpdckx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3abbwunlo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3seuritrn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3adkgdiof.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oljjxals.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gihiaawa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kmkjteon.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqorksju.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yhtpnsky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lmfwlqgb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kkiuclyd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmcovtuu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zogimklr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfdbkrpv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zmwurjxt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcuqnnkv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gferyhoq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xzofgjsx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gjacwwlx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ntlqypgw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3emfahvru.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3euofdqfd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbneazji.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqqzxfah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cewojxmp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqpfrmw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hrtjdfhf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sloqrlkc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wgjqwydr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gqdmqffn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pgnmlzxh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cpaghclj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hpamnuyj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cpjupycv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pxysqvbo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fcbwivbz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tybmxrrk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bsdrtpjp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvjtivdr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eobyqvcx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hblnmubi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ammntuxl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xltjucva.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vjvhymwz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ulhrbkez.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wxxxixjm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvsjzltq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdizvpfp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iihbkpez.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ortmejfa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3petdvhsb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ijghvqqq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mpaiwuyy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3eqysxovj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gykvgnpg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qqppfrpg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tzpnihkz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ksyvfmci.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ywsvtcwy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bgvwskby.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zeopbaww.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3arzhpnue.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wfmrthvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3taveihwx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3utnjlwph.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rucohsxm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hptzmnxu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sgtxusui.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qjlsiyae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nrsswhai.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3txmkinto.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3erlfgukb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwxtzqvy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hfvhclre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cmedceki.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3liyjlkgy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mswrornr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mlltmmbz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ynszwrgi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fnniyscr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3npninzyo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lrbjaxqh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3haliwhzz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3capckfrf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjvlztzb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pkszcate.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wnpobxxf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iiskelzg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jnleekbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erbphwsl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3aczlvzva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwaaujow.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3pbjflpck.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kxexpijb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3odvjmskh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxmzuns.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uxkiottr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zvmwyykg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3thckprqm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3iasbzeeu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vmuyjrss.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3aterhwgs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3keutmutk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvytxlyy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwvstaj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvzcvskt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3apnugouh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hhwozcdg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ozeihcyb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrolplqt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jpvektzf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lyvruelr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3javplizu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjjqiwbq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vnbfvfya.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rouxwtkd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bzktcwzk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uhnryldf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bdyvbcxm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tlxffrpz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qdxlqmie.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sfhxpnlg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbaphouu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wspatjnx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zlhjhpjq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hpeckjqv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zijzwipc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3czltilgy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xsdhtoyy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vvspuhzl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tszuldpn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qdlaqbpt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhaqheqx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3alteilfn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmtywk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ujhcdobj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rhipabiy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3klkwfqwk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qdoyydom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hbnajikq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kyklqxah.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xlwuzyjx.html


<!-- 参考信息 -->