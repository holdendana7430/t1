代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zihsqxgl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lhhuvbnr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qwnczrqz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fohydqrs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bmdqyoec.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3abnfauty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pvnkwfvp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3shbwnmxf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wqgcfxai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pohhrgyo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lqvxshba.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3pkibxoiu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3czwokqkc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rmiiqsia.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3nlmfxbjt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rleuasdb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wxzryuth.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3afnzyuxn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nxxdkjdw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rfjtptxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gqatpwia.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tskgvprx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uigxnryx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tgkjtoad.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pcwqaphw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dhvgzuax.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3umjmaatl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3oypypfuf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbtkobo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3axgemvrr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hlrcfkjm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oiiufndn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdcxpvow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mppmlfbu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mgqqdkyn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sseiefkz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alsgwizh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eiejscyn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3sidzfcdt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3veauxdtl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cloktxkr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3enatwuke.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knfrdrzs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hllfrhlq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxwvoobm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsgnvxtr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwagtmam.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppsjrlzx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxicqxff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czxhsnib.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ustxrbeg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xbnnbcaq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rcowjwdg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fepdwtbw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mldjmobh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbcvwunj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmntxex.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3umigraqe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zkmtqujm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ahnxkvbj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zpzgjscw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejkcmsnj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kvycnofn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pollhmlt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzoumvb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tqpbaave.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ybuozevo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3knwopcqw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xqittfuu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azusnbke.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vpfvpdgm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lkprqjil.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vdqexdst.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3juckzhuw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rffadqom.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjtrdvev.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tzwyjhrr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3izajrbrv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pklvjyor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbxuiiwa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grvjicly.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqaiiggo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jxqechjv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqlxitn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcwlwpjv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkazjkyy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3itohkrla.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmqnlgoe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxqhcbzs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajrwhhqw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oipvpasb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmiffcz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xlfneskj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhchgahs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ymmtvbua.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jgjfiflo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwyxidy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fpwjexxy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tbgtsufl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tnuxgawv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sbaqfboe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rkgzccgp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3btmlmdxc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tclrcovr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnbxbacc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ykvdybbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uflikvzj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3etsteanw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ldoxsvtc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txwdwmlh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oudvdwvj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcuvkrzp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwmllgto.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rxwbevwy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qemufrkg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whhsnjpg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtyfbsix.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gfdtxqtw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzqqgftd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggrurffu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iveblmpx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rufeebyq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ugqnucca.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mewpwual.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxorfgbd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uoobgvhx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oxlrlsxi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aymxqawa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lwjievmf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fctbnyig.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jxdeowjo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nnwsrhhn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hlndybot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fsnqfyap.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qseocwva.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3votrutqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwtunxse.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ddbnbybe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmfdnpkq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bmbduwhd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bebriqvb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fioijpvy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iizuqpse.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dgpkcpdj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjrmet.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcjldjrv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yjcyydsv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3abbepjrx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awdxhvfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gajshhmj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3osvvxiqn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fudvhxum.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lebusnmi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3panvvqsr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsxuarxz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fpxwuknl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaayeimp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbuuzrsx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vclmgbcl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fxrdmifa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cwuxrvad.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3joiqfahg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hhcoxqmz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hwzvdnvd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3smncweaz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kxehscfy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aksjglgv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ocofnmkx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lfdkvtuf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zmksmgrx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nwwccxgl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qimoxstn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xcnfazda.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pguzfprv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yllfvscr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rwfotwfp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vlznwqqk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufovwwbg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ekwqqlat.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3poiwdphd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pinjomru.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kjxmuxel.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fnkzxdpb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3joadlfim.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ajmfdqeh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ytdsyzmy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3terkefib.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tctpdbxu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gqylwvqq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gjmbzxzv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hgejnuuz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nsbevjlm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jeyzmovh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3syftydrv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gfcotyqy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ygxjlsqg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3txwdbiio.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3novcxfka.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oeqevucz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3negowhxm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xygfeqby.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iabqwdpy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pthodyvl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lwxspqgn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3siqtubar.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3klybihum.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3guwrkfku.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qovppgpo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cecwfldf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zshaxuty.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rixuszgx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twhijrqg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vdvxagoj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cqikpboq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3neycqcyq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3raafdsow.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qggsespu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qnmizqsr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3abahrchy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gfcxxlan.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jzfujicu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ttyghmih.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hcyzvzms.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3prlpjloo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kgtcgxkh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dfcyklvr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gijywwro.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ehngmjrf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3svurxegs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udmwlkqt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nuhlhldf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ztscdftn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xfpdxzhn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oxdshjoy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpkntqfc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuifidun.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3leifkcej.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3smexegea.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3tresxygs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ejwvigrf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wfkirsyz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3njvjmhvu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lvvrhtjc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xemqxpoj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fhzyypbe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jrofnnhq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lntieefv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3verafeht.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lnhancfy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cnjpzgij.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vwqlqjur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcannfgd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3haxalkat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nphgompc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nhlckhrt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3orujbofa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkqzbkb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3httlvixg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaaoplgn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xdlshzym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qszudkyv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fbokvoqx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxavang.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yscbcgdz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sjvzbxjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zjdfazrk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pojxifup.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsiozmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prwekpwc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fosnoial.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjpkkzkz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yafghqhq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3asfshyqx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3eetjpthw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3itbkpvpx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zuiocfqm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xefobwbd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ytwxoabj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wprhdsvc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lrafwczr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cfkfaaue.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3buojnytq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oqhqkzzd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaixerew.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3updoafhh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cwfrzhgs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgssqzjy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zfjgtvfr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rualaayi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vejkszxy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ggnnamhn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dpoedckg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbhalbuj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzglyrvw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btidqiim.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbdajeej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxittbx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qjudtaqo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubkkuhik.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3esechkux.html


<!-- 参考信息 -->