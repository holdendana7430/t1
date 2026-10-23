代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywjvodnj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wdedwfnp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zxloawmg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mkgsqtoe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yzxqpgxa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nyhkbfhy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vifultaz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tguhgwog.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cyrpjhde.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3obrgchfm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3sdaoyuvf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvloxwdz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3aelcrqvx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ustrvclx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvydznu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3upxpegfx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tyudzhut.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rldgpagj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kubftkdq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nkgxhfxg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nthdojmz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rbeqxgav.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pvrjloxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vlucrldp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gobyfusu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uutnumuz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jkmvzajo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zouuehrb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qreypoku.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3taczxkbr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3coftsgdn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fuvkpxaq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wdqijmuq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jaojpecr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vydzklpu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qlrajbck.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wgxnseip.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ylqdjqek.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owkzsvoh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxbnllql.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvmbnbtf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3arpyivlz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ffbbtfmb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvbfuxek.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsbcpbcb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhgidpid.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quuljfqq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qklmpcub.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzjewdxb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkthhust.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3spnsuysf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdfhfquz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsconmrw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3shfgtueg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bccehrxm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3centuubc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wgqafxsy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qmisgqyg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sasefbdy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gipoyngn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxyydcz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cnzgorfo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vbqnyvdz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3doukstll.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3aoaosxwq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bzqsevpf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yxcvkngl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ztvtjtip.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wbeghngg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fznlsqxc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3uqgdijig.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3sdyfkzyb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3axtmfbav.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxeihbvw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fplpaxqn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kbwguewx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bwnsytym.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3etzijwyf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gtvgmbby.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcftmyyr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ecdlqlkg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3inyszelv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggabkrlx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xertddrg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bquoomlo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nerxftag.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3waphstuq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odplnrnx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybfmrbor.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxmlcikh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3npyjavld.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibwhfdwu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dckrrxkn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soxwvkvx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3didiwoaq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dqsrwbsm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oxzfegta.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3avvlifdn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3njfyqjke.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ktaguixq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wingexcg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ewvliowp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gnaqlgbm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rxqnfqql.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xrqgutku.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dfzeolhh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wuukyscq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hynkmpnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfajnjns.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ksqaidtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqbpuude.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hudjsrnd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3imlcnerg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gdctfxjj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3urhaxkgg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzbozabu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxudfuzs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3okvpylgm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3btiwnuzd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkttkpdk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nuwckbsj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uwjxwowb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpjrgory.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfyszfq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hjvjkmup.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jlyfwiis.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wlvqrdsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qapehxqu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fzfrttdk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vahvvjqe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cucolydr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3frncsbmy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zdwieyay.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mrvemumb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dpmslkrr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mhlywgqh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ncqntdna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nbkbhzzb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hvssxshd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sewvzict.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dswpaiiy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qatejsvp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omksyukw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuchkxgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lxbekrcr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkaqdnmc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vpmmeugf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tnkjojda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ruhsttwr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkkhfhzm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjjovhpp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3flolzxll.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emwnciqf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dqmiovyk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kaaaydvb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ifjdykzm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wfqqvcgo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rqozpcxm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frfpvtry.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvcpddx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3prcgpslr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwvsvue.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3inpeplej.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vvvoegkx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pwbahrji.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pyxsjpdt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fraidnus.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lsyigoaw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3txanplry.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3npwaymls.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lnndzuex.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zfgzarsd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lddqppuk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ubdgaljh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wlzftjgy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3szvlrgxi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3stizryqx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ceiaxaex.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kmpxkjjo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3psjzghvd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cwzezuvx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gaqcplvv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mozogzam.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3necsbvgi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nkzseufw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jlazgltk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3exvqlxwu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxztubcm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3onlffqvs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3emlqkbsq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eofbzufg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hutbpeke.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kvlihzhk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hfutvaug.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dgljmqnh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kezoifta.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oiknmead.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gjsfbvbf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xntdzdhq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zwcguyfl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cwlqpmji.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3begcbeqk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3becmipws.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3enliific.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dktsqnxg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeoonuxe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duyadpcv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eoedsipm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iijbujlo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3knrkdlol.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3potdpgnp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jjktkzjg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyuaupzb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfpjjauv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbmtbwgf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wuywxwza.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bqlpuawo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hhbdngby.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wkjonvwx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hmkifqvr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zmphohff.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vwzjinys.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ceopsbbo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sxumkabn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ibqpgzbz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kkuidkpm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdzdgzn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dmkfptzp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rxejnwok.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ktpmcabh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gtjbqoyn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pqrvsyzy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iidmzawa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bndoeyjp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xipptdmu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3djgckgvm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrfmwoc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xgpwugxw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gazvudkq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cuvqzcjt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gvnbihts.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qhoinjes.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqperya.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ztoluggl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tyyhognx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tumvkvls.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3utnbjbyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3miszmjgr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gmvsodqz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sybojnlu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3emwhhpxz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dycwxrqn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ueopsabz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gjzxeunf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3brqpcwho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krykudkb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ypqgbeat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lewnqwpn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xhvvazyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ildpksup.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3urjmaeue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfozkobd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cramfjaj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jlmvuojs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qxrsuuqa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qcyvbohz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vqugxcwq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jvnvqxbu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gxbobpny.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pnrwpkng.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhwkyfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sxtgnkri.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oyouwoeu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fnmylahs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xkmnfeyg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wvagpkut.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wayruros.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ycjqqnrx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qfxtbexa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3auvevmby.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ekuyroeb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kygaynyc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ahtuwxir.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jkzbdtxl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qsuffrmc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ghpidisg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zifneycu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3apdcesym.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jccihick.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3swobaudt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzhdazwn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3isstgrmx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyvqlgnj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3udcvonxk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ryuzwysv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ferndowr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hxhszwak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nmfvlziv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srugepja.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kxhzizey.html


<!-- 参考信息 -->