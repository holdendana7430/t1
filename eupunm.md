代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lolrxwtr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oxehrinm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnriqqqf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dnyplyru.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vkysmjtf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lttbtzfr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2eivjmwdf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvgbjhaz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wpjdugkp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2avwuohhi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kexsrjzb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2unwcmfiv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghuuxmjl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pjrkbuzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xcftrwhd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jnzfsrsh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gaepynbq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mbyixszn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gcjkcyvp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2impyzqxk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2awxsqdsk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aweoxcib.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ifmdvadg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hyzuoxyo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tjgpihdc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zmsmnigr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dwqornyc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qaujbnhr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rerzofpp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ntklnpic.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2omyicjta.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cckigynh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uhthicso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bcykwzfm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ppuolvwp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gitzxkbj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nexfkbzf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2goomdxjx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crrtdhxf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uehystzi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iaebsozb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qjdxmtcz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ufmshrvx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmyxfuzf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvxqtcjx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbgtpozr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ausvcufs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqjxmass.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjnpkfp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytwlnhmw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhplzmog.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhbgtkcv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntqjvvsi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wbnujymd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2uzuxtrhy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2draobsoa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2udtzuipg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2offyoljk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2isgzshkm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yxamycfn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2npbefbdo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kdnbmaeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fzaibazb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2inzpglmm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qhirjmep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yqelhltn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dyccznrv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ygpelbxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bfltxgcv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2duoiosrf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lotbuvco.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhevevll.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2itadcydm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxkhhjqt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gkbfplsj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dxoojrne.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2brpcmzzg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nddcubjy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gorrvpbn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tasgvbga.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qrzvjwgy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kvklkkiz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btfcitax.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djimethd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gsxdknpd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzfcyhuz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uepzkqqh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfmnvaqk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqyownmn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czxgzoxh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycrvkffz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrflfhqm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kksgiegp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdxopgzb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfjiebdw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fijlkpoi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2suhflrji.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcdbhsvo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zvapycmb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zdirbhpy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ibcaqpkp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bcudscky.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zgplsfov.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2etiybenb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hftzkfax.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2njdkoafq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tvldlymy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jhukteds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whpbpxeu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ksksiznq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksadavzj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2adyxhdwf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wyxwfxvq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lrehytzl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2suwoveux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2welmytyp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2elvpfbsb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qiotwgcf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlqzgrwx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wivrlspy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rjnexebk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vbzbmsam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayadvgxl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vtupghxv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqvfflju.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kvyjvegu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lcdfedgu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2daqlcuia.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2adifyxpo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kdkgsyte.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lepnqlgo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ijkhxwwh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eoufopjo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spdobgje.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rzbqigao.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ntfkuwhi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kxxhzwzu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nnuebetx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwxeemwa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bppfatzz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqorunma.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezobxfxm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2adwfqyrs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vazkaqby.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iiumdvdq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2njdlibif.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bcvamonc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2iddxpjwg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ojlkdmmf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zsoqbskz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rvaynaya.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekbcluoi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uehvyibj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dnauhdvw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eblmbosi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzsrepnz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mqyayjra.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tgrxkrak.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuvhiuqg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebazvgsu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhzdetf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nnzeiosc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2liwhrgmh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qvmacumv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tuvvtytw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2anlflwvc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2udbwbnva.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nmlohdxi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cslpcvlz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jiccnxcc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2moqxhwaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2opvkgosx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fytannbr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qaowwbbt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2iridwltn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2epmnxrhb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xmxobdcp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yehfchbk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mgobjwwx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdjmuovb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2miqzfalq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uydtsifu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqtgvocc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ysfbbvvi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wluihlcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytpwgmyw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2egeaieee.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2biwchhbe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hszyyugk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nhpuopog.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jedufsbh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2iexqriey.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2izynfybp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mtvnrzfz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2svdgfqch.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ylwytkht.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2breyuvhm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lzotccdi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mwwcyxjj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2blibzfai.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ipdyswxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2amxjvexp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yfmalixv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nadlxzic.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgayivbx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khitkdqd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxjqxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nbugxsuw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bzzodfpa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cdoisahv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oyajlhec.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kymkpndd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2culxmdoq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfrlpke.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pnokbzvq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2timzxyng.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dsmslijl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmkpazfk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2spzjmaff.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fnhclnip.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mmgruavx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kgapzjma.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wdoxfjfi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xyzahvfd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2axfkvgyz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qqkjoaoi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gtpxfusv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wcnmiaav.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bniwaecu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jgpoojbf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zmxqzjwd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uihpqpui.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cfbdzloe.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ivsyjeil.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqywibc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ykcfqqiq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2frptnaba.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dvnhtdye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fqiaztfr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmsnusvc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wuppikik.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kcaiuixa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2haknamdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2izaihibg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2blbjkxfk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2leadpzzd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tmdkeyxm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tufjjxfj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nulcfbxn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dniujczu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wlnbotnk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nwrpvfwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vmnqsamt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qtrpuwht.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2abgrncgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebvamzml.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pjjsynrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlyxwtke.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xmsgrzcb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xogpoyyf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gpwifyxa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2euexkkib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mruwylng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhygwvhm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gminnrav.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2sxxgrzcr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfziwzv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xnqjiojx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kofurwyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxztfqx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyhsztcd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ezxmvgvx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2swuljfpm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vjjxupwm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2upallsrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2folcrwrc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ytwzjdmy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bbwzruxc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fxjstfkg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qxydhnlv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ucsntdjf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hpdympnr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rhaxxsyk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kamzxzxk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jvfgukor.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifhxjaiu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2srzkdsvf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lzpjmzqc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2anlllcjs.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2auanhcga.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uxxarsln.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mtwskdks.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tsokogax.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2awhxjtqc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vqawfbfg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pvjxceck.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzabkoro.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fvwmqwiz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2febnixln.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ahkhgtqc.html


<!-- 参考信息 -->