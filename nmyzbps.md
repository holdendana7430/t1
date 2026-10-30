代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gpqdnllry.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gpiazmwws.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/geoiindvo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gibgzpwga.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gxmoinpjg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gnatzjvfs.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/glmzbhril.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/goaxzbhzq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpbkfosjt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmlqhdjtn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmxcfdcfs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gjdwaowcf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gutrntwbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gesdestgl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gyzebsufa.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gqicbpflc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gajifuvti.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/grekerdik.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gstxorrgg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gcyyzcnef.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gvlnhyzfo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/grkuvpfbb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gsijcnvtt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/grrnwyaxu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gzjzuacmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gnhvvmfab.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvrrpwxml.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goyseofwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmkegwsjs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gifnpdoyf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gcgaaafqb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyidlkigq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaehccryz.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gzkjpvnxf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/goqlhrjqf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjxcebneo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geowazsso.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghsneqtdp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glnmmrdvz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqmlruuqz.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gixbninqe.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grqectzeo.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gcsfmmlcu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gptiyoftc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gvhlzpjbe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gbiqscyoa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/ggeqmcfkz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gfbtogerf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gpyptrhan.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gjlwreggi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gghssoppo.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/grxmuojwc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/graecpzzt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gurposcyo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gknmdhfbc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gidypbcgz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gmgxrkbeq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gjczdadsj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gbksmbtqh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gcytchibw.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gdpiqxukc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/garuzokbz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkqbhierm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/glhljsrsj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gibsstvkg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gonntmivf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gdvedomme.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvfglrlmj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gnugtliaa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gtbfexhkn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxaqpwxjg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzouzchsm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfpakoeip.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcnbxernv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gnsmdcagn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gayovqzxg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfvfunqqh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gvhrmubrk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxfcfef.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmlhitbpd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gmuanrafs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyzuskenv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gubkqyuuy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gotpdyzit.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gdhpobjhp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gitmxxqko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gxbrgskjq.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gzlcqbfgz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gvgxbzfzq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gnmklublx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gtarzppjo.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gtowexuyi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gnpegdgvf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gwfvraitp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gsycukxvo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/glkxvltgf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grhojbbay.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gtptgtffx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfwpklxmb.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gnkkacdxh.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gapndvuxz.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gtbwcoput.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gsrbnmrbq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gcijhgnmx.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/giiuhpwfa.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/guseuvual.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gjodnqkdk.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gltizokbu.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/ggeydizwi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gdwkxiths.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gigurmxdt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gsgfxtsrn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gpnpumuak.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gsmidzpia.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gjggkzrfa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gqnixmbat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gqlhvefnv.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/ghmikrrce.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gpvpdgbgc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gbixmhhbs.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtslgshhu.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gdilatnmb.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gdnlgyvmr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gsotsfmoh.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/glvdhuiwl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gxfarzcxy.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gdzitagll.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjndomnmx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzgvsyoxb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwrzcwttd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmrtsytjc.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/glbvplbvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gfuthlbwt.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gnhvntwme.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gyxcorfqx.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gbbknokby.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gpgvdwmbs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/graqfllcm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdvhpqrlr.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gccejpyoj.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtykznhne.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gnwwjmakx.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gnxardihn.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkcxrroat.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gxbrqulor.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/ggucbvlly.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gagjjhymi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/geqknkreh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpauhmitl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gifjqjqjk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/ggqeceadx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gdugmoaxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gkxrxqrrt.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/giaqigccy.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gfjvdatiu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbkgzajzb.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfmglxg.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfijvzscu.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/grstbwsyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/geiaeqvbg.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/goaqugdfj.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gkhmaofpz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gwwozykyk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gupnpymma.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/getjtnxky.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gxgizzotj.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gmjtdehaq.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/glegiktgl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/grlayuatm.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gdepfnrmw.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gvgjbqlpc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gfxtwvdad.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gnvoeudby.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gscleqwvx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gxguolsui.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gsbyvsdjh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghzzxsole.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/guziibute.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/ggrkfwqvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gctdozdoh.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gsqbbwiku.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gblcpfsts.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/grainpkpx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/geqrtsxzr.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gufkdwfut.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gdkwbxmrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/grxivxvoe.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gcwixzrzr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/grejxleon.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gdvrbasfn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gqwoisven.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gulhtdcto.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghlojqtso.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gztzgrmrp.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gehhvdjnk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggdcdbkbh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gieubstcp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gonrvftjl.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gymzuidjd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbyleyxhd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/geqynwhym.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsctsxbng.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzrpyiqxd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gihuxzstn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/getoatyhq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/garuqtgrq.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gbpspmpxc.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gqolvzqsu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gjrlbkxfw.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/glhtxxoyk.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/guontfwiz.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggmswnsyw.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmkxffvok.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gnaynockz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gbxudcjiq.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gbfgccgem.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/grqtbntnh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gkqbwrgiu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gchgzpvnf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gcemtpsbd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gwagvupyi.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gaxrbkues.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/ggrmuupdo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/giowbkprp.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gwebwdbxx.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gbzcfbbbr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/goakqigfi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gdakfxwyy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/geujkozwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/glecowkhc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/geuogqpvy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gwfmemwos.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gyenaquka.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gailxnool.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gkqfymlng.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gpdakxpyp.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gaxkwzysz.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpubsrqui.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmsjtjocy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gloftstoi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gsyopineu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gkkgaxjwg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gitdbutaa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ginlfzisp.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gldxnijof.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkczppzkj.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gqkxotvhk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/geevxgofr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gtmjjgmiq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gtmyzvddv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvrzetcbd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gbfojsnwe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gbrsvvzln.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gswcurywh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggeoglkew.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gqpiogngo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gryrojsxc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/guuwjsqvo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gizxldcic.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gogswutso.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/guwwuszxc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/glwfkpddt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gsrwlhcuj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjjxwnlwg.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gfnvywbho.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/ggjmkjxnr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwvcsawsz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxgjmzliq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmdvallin.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbvphjzae.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gstgxjgjv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gvxtnboqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gywjnbaqk.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/giislbwho.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gdvjkortp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghmmhbzbm.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gmroxeuuc.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gyncdjmcx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gftfmpocr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gcgpbtlee.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/grrpaxvtf.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gkgkdndyx.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gdyhvjjgh.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gdnrmmbnj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gqtmfjlfy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ghhsyrgwg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gawvxtsro.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/geqtrhtob.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gjbahrzzs.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/glzhjeemt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gvpmsetlb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gqsobpowq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gnxrqwycn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gqfpsyjkd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gzhmuvrdn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gttqzajzq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gkdranbww.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gbeltaexy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/glpdsypev.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwkkpffvx.sHtML


<!-- 参考信息 -->