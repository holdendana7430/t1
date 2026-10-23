代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ajcpomdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aewazjjy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ovjeyqwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qiwronfk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsrpaqta.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cpevxoed.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jgdnnpey.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yzufrpkj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nzttfgkq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqnaxtfz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kmhrlpwh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mgomnmod.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjnvdmjo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3luyovfwy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vfnxgdpa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fntlhuec.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xvijsjtq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svaycrzy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3andkbuxj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhoouahx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ktkhygmz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptyrbdtf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xjgkwmnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3paijbbva.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xtuuzcop.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3scfgnsje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ptbozvda.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3enogywzl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ofngkogn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nzodwdwk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3alsusdpx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ivwipcjy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rwjqkgfb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kdzpmqdy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sepbbtsh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gldrnnwk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3llveelob.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3chtnrfej.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bwykhplu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zownadci.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnmjsi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hysawlwx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brdtaarg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbzoeodz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igkxylia.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtvamrwb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zugvcjqd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3phupqtag.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kahpktxn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gkkpjycf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmxdzuzv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sqrglzgd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkwlrpjl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvjdgppy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ntcudbto.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvxyzdxl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3votdysaj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fgplgbvx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fcwbhgpg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fcbmuurq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3diqtaeqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yqzteevc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3frynuqrd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3njhvjjid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wpktbgvn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dyhffxfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3adrkrazc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3anigpzsn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xekmfavx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kmcmissv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wcuioakg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eidipwnl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nbrrxrlj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3amecduup.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dziypwck.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pnficejr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wgqwkmsc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqmserov.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avjmdiew.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3csyuggcp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hkgcsjlc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rfohpfsv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pozizfqi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbqqcpyd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gtqsyygz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ybpbecyw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukirsdha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vosrvccp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgbjawtp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwmmiedi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nyuwaqaa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ictmqdhj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxjkucvw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldcmwaek.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zaourdvl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqpkanzn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dtbbzgcc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twyiwrxf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3leqqfksu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3awpdtkxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yrdkcmas.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzbkmwkm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3logyvknw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qrvekofz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qgcqjsbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xnriaipn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hhumuvvm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jzvtxful.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yuffcefm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3taamqswq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fvirjqrm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rpwquvcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otmnxyeu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tqnmhrfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aueeqfqr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fvbwxobn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qwbuxkna.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3scmajqem.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyzuqnvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ukiesxtv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hkodcncb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ennpalnu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3oxkyhnur.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtjarbip.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihgsvwnh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ayhfyhso.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfptoovm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pebqadlz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaxawdaq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hoxduuxx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3eztnlcfc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xydhvwzg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqudkzar.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3yaworkcm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3aauuqhdq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fagziomu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3spsoycer.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vpoxrqfe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zxwnbpkp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3okughmam.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3enjelnpz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dzeaxjdt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wtfaazuh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mznmomlf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zbmhwcmz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iwrmijvi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3agcqevhd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfgvetcz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kljjcfok.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckcmahlx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ybfopdfq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3boqltnrx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3byvsefti.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcpvjhlz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3czogzoya.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwifbjkd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lsncdbrs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nggbebjm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mlcrpacr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfylapml.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3svprehqc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rrwcyvxq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkoagwrq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xxpugxhx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfheumr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cksiytmx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vphafrwr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwhjkqud.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3povbmnpz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ttubwtgi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ounpsntq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fpztfjkb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sjhgtfko.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enzhvjfe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qxheryfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xgbpeywu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gklnwewy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qfpzebig.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ijophhqp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oxoxwchp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhcyslhx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrxowscy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qmxwnkpn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3avpzglse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qkpoovzi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dpjeotfa.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3klltrmwh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hsojuaqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tjrrarwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3degfhdlj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mtqpcbnc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmimxip.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnsenzym.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3asyurjkw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cowdtmjc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqeqpvd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3thzybupu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ubqwqcti.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zxggmnrw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sfaijwbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3psbaivhq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aurqqkiu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3abhbnvqp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xrwvdjos.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3iouoxpux.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ceyzufqe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jzlxkcwh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qbhkfftq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cddwbmql.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xwslnfgh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lpoowdeb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yjxyhhhx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iunotgju.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dibfuunl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rmbnizdd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iwmgphzz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3epfmlhpl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3skkrqsco.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uxrkasjy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlviylln.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ngvtdrxi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaexoqoy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jraxrsbw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cfkpdbhp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rjedgoeu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gdzwnhim.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gjvitayc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3clqkgzhj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eczffthb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ieuncvba.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kiiawihr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dqctljgs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wyuhqxhu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ezkdhehk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pktadzic.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3muksytks.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rtyirymp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btesvees.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bybaxkfo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3grqdinsa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rpcoxbdu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nphvdydm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3pyxxomto.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rreimfyb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mbuydnyi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jevzhaim.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tfraebaf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cxsstjgj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fcilcite.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zwuesgfk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qkscbziw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rpfotkcd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3czbzbbsr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgplybke.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iilaeked.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jyzrtwxu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3akjklemb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gjlwxqht.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zcjskejs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sblywywz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wfymuyaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uudwseoy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3odezurtm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bljezojg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nsfxybdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nmmpgpit.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ehrkranv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uslcelva.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fjbedkgm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ndigmsog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lpjmeocy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dzkuwzhs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ctrunvme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uvystili.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lsadbrhe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3icpupeie.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwvabyjp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cfbqjzsc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3uixemhel.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iknzxnil.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jvweddgz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vdptcgdy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhiuqixk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vlrarzyo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idtfwrgn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zpmxxhkg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gufkxjrs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3msriccpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cuolpsxy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tgjzoofh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vujvcsga.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3omdjlumn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lawxznql.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kceufotv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhbnhjds.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3symvupcv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3oicgxeap.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hsfmztqk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqdccp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cyesylqb.html


<!-- 参考信息 -->