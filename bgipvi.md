代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccbjwqox.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ntxbslts.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2veamkqtc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hygxlikc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fpkrmogl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zuuubgid.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lezfduka.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wiwnfxji.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gewuxmzl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rjoyqerp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fqyvwzkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbtwvu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fecezkzl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzhmuohj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zztvckrb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cpbrrnts.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dqktqrht.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vlqfhkpl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zboonqit.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rroqvotz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2trnntkpy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xkghjdrc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vqyejqug.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kaxxuvmx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fqydohzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2idalpdug.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xqsnvbjl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ixnrgxvv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jwyrojpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nerrqzxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yqryyavh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ojbxlbxq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2axxkeywq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nfohcojw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2sqkvicqg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hvxbwdit.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2utyvaiwp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ktqwqmmv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvyfjytg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhfwjgpu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foaizahf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aavpuwpc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wqurvwix.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asfyuhtn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nryuskje.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yabnyquk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oneksfnf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shadnwha.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2daweejjb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmgagjyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ojicykro.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffdpqqpw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prsomyxq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkcvvkrd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2trtifton.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ztbcirwo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tnulootb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qyrcmjhf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ojjkgfuu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yihojdbr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xcuivizs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iaysqajt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2htdeflxd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lviumlvu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tucsdjim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjtodtua.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aarenvid.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nzbbbmbo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eophdffr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jcxkivfq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2faspwgzd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xemjtise.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nvlyulst.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmzclscc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2onrmexfn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gfgnridx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ucfqonfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qiejrfsg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zjualwyd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbwoqcan.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ggkaguvp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jjsxjvpq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yupqhflz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlixqpxm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdniqqwz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2asblilnx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oskvfajc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epjmhwml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxepcqtq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzlskeav.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zdyveszx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkvgvhuc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rysdteqb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubinahrj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aglfdzeg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jvkzcmlu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fxfjkqgw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlpfegcp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yaidchdw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zihzdamr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdsnakt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2txzdboba.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bkdbiquv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jfgjotnj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gjzyfrkb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gjwjckyi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2sjyklosb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kqirwpvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvllsrru.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2juuuumbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hsenycch.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zchvxknn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mlyrzswi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bixckmob.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwjhjxde.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2olasmxad.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jfbaorvm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tkdlyrtd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2avvqzltd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nibfhnie.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2khhkeneg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xmoahppq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xumnsrcd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddpeorri.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqbkhohm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eqfxptyf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcyuznm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2roosorgc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2emwgrekf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xtrdikxk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tbmqljjf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xbicmmel.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lbqaevtl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2szyckdpj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jtkfhpoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qmljcqer.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pisgdtyx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qkewsmxt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ljoejywr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jwgylocf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhjvpur.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqjbhzd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czsarmzo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iqnbfgza.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xqzobhic.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2duocuavq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nonbvuov.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ikiugizs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tkiimkey.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpyqrlwy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2olqdvzaj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2erhimhop.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrhfhcfw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uqivvsry.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lputndqn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnizrsoe.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zhmmevbi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bljagzgo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfrztjn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggrnidyr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luugmhxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhxlsmw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qlutjoqm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqykolxi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dmiqdurb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jecrtwzu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rirnhsgw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbpnxyfb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ncserxem.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2numljmsm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vrbdtcyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vmwtwtcs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gphmtqim.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fsupzuga.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xdrpvhoa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2shfdohjp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxbhdhbd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2brrdsods.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2crlfbrub.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tfjkarur.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2svaodquf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yicbscsw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbkwqymc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2byknxwbq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2omvhehhj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kxxlwqoa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2swffwkkg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yojgkwbc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nqjwndel.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ykbfgwvg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xzatcikw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mchkgres.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rufcfxqr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uvhggggl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wgezureg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uhnwnrpu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rgtjfixf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qeallgfe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xfpdsrhw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zjisftbo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pdnumydu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fjvbkpnd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lficgxng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mthvxdgr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftakehzr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2frcxonxk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebpywyrv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2npntmcsb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bxskbdby.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kktmjgkr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2stmtaowr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2huacjxsn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mplngiko.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvclhla.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrykvnx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vbkgxrqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2htiyystf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vlmctgla.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cinooago.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2exkkahso.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wtfnaukr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wfstcvel.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xribzryj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dcrzrwpd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uuiqmbmy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zyksiuko.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ywazntzi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dkecajnt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vqifvypd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wviqakut.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fvcetlub.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rrpdggnj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nwerphfk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ophsqcni.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqcgbgx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pybelnhe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fkuzvxzg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fcscptwb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sbnafugk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjfquid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tejmvpng.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wyzinszf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fpylrpnf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gifzvqjc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bnslzmfx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bxzrapiu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hmdrpjnh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ohvxkbny.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lnwkfgxm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qcmlevxa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnacfvdg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hhyyqdls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mmjcrrwl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ccaijpib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2flqwqzuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtiiajkw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ewiekpnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufcrespt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dtzjosoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqdwhtz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2esyxpjcn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gffznpyu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wetiaotj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lkiizorq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pnjukeve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ekqmpzqm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2joxxhbkb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hxaaecwk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hopvdewe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhzlcwzz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fyuqkaso.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2krprigbn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gfcmcfww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mhckwfzu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nyfzumay.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zypgjgav.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vxpuriqo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hfdykdjx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gwfgvjqz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oqsncoxw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ybvqdzgw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gvnecrtr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zplykzos.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qutgpslu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hbzkmzkk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zlhqkgfj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jtciughm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vhirgynz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2veqbnkeo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bamkvfoi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkonpsmg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpbfcog.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2uxfkkuxv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kivrjrbx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qhmiaiue.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yrvhxraz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvzlruvg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ngmyvych.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dbjzmwbw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywbpjlkx.html


<!-- 参考信息 -->