代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cjfvbbtm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2shbfpdkl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcngckss.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nkhyvxiq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2befuzvyq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rdoakqwu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rxnmkeil.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayajqvgp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aseezdwz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yehphjxb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wpmdmtku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lvuoramu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2levzwzsz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvsrbzyf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qbuvmbeu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvarctmo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ctkppbry.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ukjiodue.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zlpimwou.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rcnlrvby.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ulmhbgif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dpawiemx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bddpsyse.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nmhnowbi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mdkbpajw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pilrgtvg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sekcpjoa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gisjwjye.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ithxgoby.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kvobtkkm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xdmvxliy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gefgmcyc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2evfunzfe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sbioczfs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzcqkymw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bmlemekz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sofwdsgd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nxpbqghv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kmmkdtxc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jygowxoa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfsbvnss.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wvjfxcqd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fzkigszk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnkhwll.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gecuvkvk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiawfagc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbemomcq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhuareff.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcxkgoac.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mubztzcy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mbwdtdip.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mitxsota.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptcuerzk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wumnygkc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tpyyysra.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlsfxhv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jjoztlgt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ceetuvdk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wauaxdun.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jeefvthz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fhsopegp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hajfcdkp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zjavbpnn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qkfqdnhq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mepafzdg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkryzepu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hfgcxbrr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ykfptldi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yfxggmzn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2snusjxxi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fvzrwlhx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2prlddxml.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qzgyuthi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yeybbncp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2incnffgq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wmqncegg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ttmibupd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rzmchshh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ydhxdwof.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qowvcvbw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2oxehymgt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gmmnodob.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmyhvncb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcnxaqtl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfywadvj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oklaelwr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2eyuosuzf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aocxvzwn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpnrockt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfmlyokb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfmyntbq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bprnncok.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svhifipz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvdvvgzd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yztxdhgo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tihlqivz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pmqyndir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnnbssis.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mqnhudgj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rbwauqdz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kehtirtn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gncobhnk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kvcbycpt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uccreffd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tofohxiy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qplrayqt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oifijgsq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2skarjztx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkvuxtsb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2msylohmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpsqppho.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sypikzhf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2odssesas.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2njoqikdx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ceuxtvjf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnczhcsr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yscotoyh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xpmnpbzd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2aalyextc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brniaaqd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pondjbxm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2odumhyog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvodjrfa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jsoobwrt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jnunjlix.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtazynvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dacczfok.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxwcfyql.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekfsjaiv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hueukvni.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aumehnip.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ydxrshfx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2abfoxfuv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kdrfxkqn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jjnizdyu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ptsvrdrj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zmrquvga.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hxaxohiz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2iaccnfzi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2djgscvrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2arljrxqh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2beihkijl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fugtdbmt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktgpihty.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kfmjmnoq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ynjnprsc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bmxxhntu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2slaujqsj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nddxznri.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nixwzkxu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2clmxjyde.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2auepqzyr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzhlizmi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2etughfhp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoykniko.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhgsbpqy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwpatzll.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fmniglvi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axhvnzpi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbwnzjyw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nqkaapln.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dlsmwqok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cemzfytx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qamdpdav.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lecxzjcv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kejkadit.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sjtmzwvz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jmpiwgkn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kznqobvt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qkjwrfup.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mqtwymar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fxudwqpo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jfhinqam.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pfmypbjj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dkghccyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ywotxvmw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnbwawgw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbtyhesw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2siihgwdv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlynobal.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hnzxmgim.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2eplrcmfl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2khaflmku.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2crrbjclj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zsfducbm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyimdlay.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sdaakjbf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldktcasw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lklaytqq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2brbskxod.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gtkvyaqr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmrdkmmk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zzqdpvuh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xbcvujmg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lulclday.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kgftiwmu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hpxgfxyl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qddxmghc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hqbevwbu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iomluuld.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2virgjfit.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qdhkbanx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kuhuqznv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vguzuady.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kxvclpoa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjofhjco.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iztwiciu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2serooujr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tcgsptah.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hasagqss.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ymkmemer.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2adngodxx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2byugtlau.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxnmgofc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2htkwixxl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qsswvqrr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qwgjowga.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndxlglxm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqpkptpy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujolljwl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vduvsdlf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tddxukkd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jjgkdrhs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mmmuyrcm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2byfcgdfh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uxtxdiwx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2owgsiptc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lqncfagm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hkvcurdt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ebyjyqvj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uyzegouf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2aukkaavh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zsriraby.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2klwpseog.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2voqswcas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jgkpnush.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mnlhvvep.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zbeyozan.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yizmylpv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jpxluein.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ykizvolo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pzpnlbgb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xsbjwjmr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2sgprfykx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2umxutgcy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bktfewkz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hcqbopkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dfnvtigm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2elixgfkf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqrnafo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bruzlfdu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mvfarnxt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xgojvpor.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nlidzsyy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lwlfshch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tutihhvo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kxvmbrbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odcopetf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fkhnipfq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qrefakax.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ezvzmkyy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2adqenjoe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyacezwy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vrkqtpnu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rqugiipn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tcljulew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qiaaflhe.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ybpaywrd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2caoqmtjk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bbjzmxes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ajnumepc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wgomeckp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnootoi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2keswibaj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxoesaym.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gojteqrs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2twywoeqo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fizlpalc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ovhatdoo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ozvoavjy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qwueaolq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vnqovtia.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2iluuekve.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lljmxrnx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vpgygifw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hpzjncwf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gptyuvsb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnqjxtmy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yduthrqc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yzkupllf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2micyjqso.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2krgpilhx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zwuipsrg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kswtggra.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fkvwqyiq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ervkbonq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2adigrfla.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2siljzawm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjfoofhn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pranptue.html


<!-- 参考信息 -->