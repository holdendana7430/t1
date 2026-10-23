代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3whnasqrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozmbbwtv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ludwffuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clqiogbu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lgijdpjx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nxrvhidq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vipjicim.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3npoglitb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqtdlrg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aedhiwoo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ivhjcalk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oquuemwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btzbbwyw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzgschuv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gtvnyrsc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3knytgasl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaufxuco.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bpdisvdb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xxiraftg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3eolmfixc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lxsvrvas.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpgelpbv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3coxzbagm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ejbsrtys.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qjaftqgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3graamqsz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ckodlsco.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fdszirui.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kpwwfskv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hhxsnmnv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ubfigeqh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfeowjoy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bzwbbpac.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ablltmdc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kurjwjsg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ttlhflyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rebvaush.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tdespyuv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gujpehss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3orfeogut.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ybxrqsux.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lakoitkg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wtlkqvmz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnadevxe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnralety.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hvqkwhty.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtpupxh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irmbhnrm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bssikmyg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xjyhtuum.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vohozpym.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmafaseq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhegvsuk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkrckxgr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mkoezaac.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upeyfmib.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbhholhd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugphthoe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hdelfvvp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjhdryn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fmzeybri.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wwisbkan.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vvkvpnrs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3svmwuvon.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vlsaycrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bxtsiatz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xfmoafrd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uivxtacj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rezbiodb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ahxlzlmw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dzctbvkq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qrcvqcdd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pgnlemzq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdopaaa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xncpzkds.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ybiaefjb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rfjlxarl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvtejaqu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3grbiidjf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vebwmsrn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zotacsis.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qqwalyjf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ixtfvyzm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzjvblzm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bnjlfvze.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ycpbnwpn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mspidpdd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tmtifwoc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihpamdxw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmfjwras.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3geihclmr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mucmyrtu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtrxywk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlwcljwh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3skxgcwqd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaezqbdi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnkhmwcd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pexxecai.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3turxdeba.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wkgulscz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qgyrvmos.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hovnfchu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nbchblru.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cletldwt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ulnyufhq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fdtwkjty.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tuqixsqw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3diugvnie.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3inpectau.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jkzyhnft.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3cmqxnkdy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ookvqibi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exrpaxtw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sptdjgdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auygkhah.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hrwmejxv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yxjyvwby.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3stzltquy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ckiaiukl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijfzugma.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmdlyo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nswkmzmk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hndxvxcm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpbtjqxg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ihuejdvi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hfwhyzyi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kayewcko.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfwidemx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgaekigs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hmwefowl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ffdbeixk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qaphngua.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wldasnuk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lsstnwex.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ynpyykkr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fpmnjpmb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqofbtie.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3imgemtqn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3flnplduq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ossqhzua.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nmyrxvff.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zvzjfaxg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rxcezrhp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jjkxuiic.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aqmnnyuv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lqectqja.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euipzqbq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bpjgwuar.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uqqsawwz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3umdqxjpu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sioblidl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3flnejcki.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bqyznmma.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfmusilt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsnezxpb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uzkrejex.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ovnhoccg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dgeanywv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kyohkhzm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nymgneez.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3utdjwzrf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fnlshjon.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkuyqqeq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rmdbjlep.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qlaxgvis.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kyfovgsy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ukkdmvcw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wkgldnzv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vzsnocwm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fwhxwtbh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lrxipqta.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3isdtoheq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjvcrhwl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qoglvvqg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vzxbalnx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hvuhthun.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sfxftbfp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zwuvykcs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gncrjuzh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lcxplbjf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdeanxtg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ramqikux.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcxttqwe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xlgkknaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ofjgltaj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uiedqfvz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3urzpkbvf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tfwvkncl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xpealhey.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxkhvwmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fxqstrxl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3otvszrfz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ltbqvskb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qoqyijlr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lbqoiiei.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tqgmekep.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dfhpxoww.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dkrwdduv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3izkhqcbj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xnpcinic.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iqafdvsv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pulwffrm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3iuiseyfq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rkzuowgi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3suztfxms.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xnyhxfug.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qconwamm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qssyzqeo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3niqughap.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3egdpqrcj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcvrjeiv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yzyshavw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3unlwtyfx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xabxbgtp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tcjyxtnp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kogtylqf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dxyughrc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcijuavw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmroqeif.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mglzvqfz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gtaqbvhd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pvnldgfv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ehelclxu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tprkxhng.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcbutgq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rfllubxs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3beenyvsg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xwsheyob.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3auvcshla.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uobrrchj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vdhslzra.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uaeihirk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gdtbuvqo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yswontwq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3eokasjnc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nrfakbve.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3suixxqnz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgahuqjp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3oxconjgo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nhkdbrif.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3djkimvho.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3uouztlau.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dmkntyuf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tqrlwpdz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hvqslhlv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qwzepudi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ujbbdads.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mdthbifg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3onyqgrkd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gmjgamdl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gnwtqdil.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vffwxemx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwlmdub.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tmbstsad.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzhrgrmh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qhaczxcb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mxooddoy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3upjfcehg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jvhhoztk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocsbkxzw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ywinkaab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnczkaxv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3avrziopi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zcrroxau.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnfjerzf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mreyhzdy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kcjudeur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lturtwta.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kvzqmevi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjcmibco.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vwtsovsf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ennxdjkd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbyokrh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fowvhurq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfhnqdrk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bidqxirn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psolyfnr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yonnrhaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3avaqbsve.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufcfjnwn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uhgyjztw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lacejvkp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3axcpvakt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3myntvwof.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rjhnixcr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvobixnk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3aduqnrad.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ahwqhicj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3peprmgdb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqrajctg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ehavtgrq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vewpnbxv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ehbkrgdv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlzxysat.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fhiudkvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vulgzlhf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tpuypzlj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvfmkuyg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ufqonzxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xmeiuawq.html


<!-- 参考信息 -->