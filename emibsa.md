代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozkpkkep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mgootzyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhhalzhv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hzynqrur.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lvyewlex.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzgelksd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cuwmglsu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xaedtges.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sgneeodl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3efhgbrfr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qrjcoscs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hkkkkqie.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydlclgxc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pntmwkne.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3izgzncyx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iydzylry.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sknecbhl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jajqjhfa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qmkhacvf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ujpvbkpv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pfybrveg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sutfmkhj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lbnnudik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rpvyzyen.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nxblwmjr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xxtjndiv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3auisdhoe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fivzyfto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rburdxil.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nyhkvmpi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ttbwnazg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jwlzbhje.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gkusbxhv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dbphelmu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hvqttorv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zsmajdgo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3begflfmc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rmalyvdl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xoqxamnx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xforrzty.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqktfpxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ytuxvano.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pwrvapzl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfnofxvn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfoxddzk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3scfwqdcv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjweunvf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctstnxse.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddirdmmg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwkifjwq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pecnszep.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmupxozb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqgeeflf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvcusqze.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jmjdbvov.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jtlecyrd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yizwzqny.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3runoxzhl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3asoczhxl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3edfbrukv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yvxfliyv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wvhnnrya.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ucnxwuty.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hbrxphcr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bmqaooph.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhbevftm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xkxobvup.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sgykbcua.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yrdprgpd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qaazqcdk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxybplf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wecypeab.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sivgudyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcyixrzn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aqqfzdvs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qiqehlax.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ipztycgz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3khgcvsew.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xzjhfmqe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzhhfrut.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jrduduvs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ysqacwwd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayfhkves.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zixzmzur.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkwjsfp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjqruyow.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ffevrrxd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgsyrwed.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imorampr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpyshymx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3srmqmsqg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnbhlevf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3doalmlsg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqbxabru.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmmksumb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3btohktyd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ishmrysu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejthfduc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vtvbidgx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rlhsfmdj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yjtsgobk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fkrnijjq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3sbieggab.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3snskmhww.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mopaezzd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3brznqhxi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3soleiuhd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zskfgsoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjddqrwu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ezfzfryi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xztccakj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mhpwpjqt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ybptebix.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wkptlubz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqncuzeh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sbjlgfxi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfuhppvz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3puynuevb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hquqzhua.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jtyartnr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xjetttvo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3okvddcwj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srnfnacd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oiurfpls.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3epebieie.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lqmdofbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3znrvtyxn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3upyuiqrm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3akmnudlt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cbughhnb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vaihytvx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zzhvaste.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fkssjzhs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rbhviolr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pirwsahb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jlfyqgof.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mfxhitwp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jvpmoapm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bkxkwfrx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3irxmajko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmzeurcw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aazpvytn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcshfotz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfrbcms.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3idkwijmb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dgwnskju.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fldeuocb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kkjmhdyw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fulintzw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kgkftpse.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpmkzwgy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fyrdwsdg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jykoaggk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ruoqhqfn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3myporptj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbctrrfj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yslmekth.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cferabes.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fgbpccex.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zcefjxik.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pbofoyee.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akkzdkqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vkdoufms.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pquwofdl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kcednoyk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dogulmly.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cfockvpr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3twswjkju.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oxsppzir.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wwlidmvp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nbdjolje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3myaneujv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mdeawemz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hqnavmkq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3biqxgsng.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3uzqiyjbp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmgiwndn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3afclnadr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dskrtcud.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hdqipsmk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pnfodjrt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbkshotc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hopowpxf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ewxxuebt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3znxwbwby.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3weauktvt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bcnvfycx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3txdtacxx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3itepcfxz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhbmwqe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hkmfrlxg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szsaghff.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bkvdtmbg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ikbljtzj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xxftftpa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bikqhywh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jjoovanb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tpxoagua.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fbmsqexk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ssinxjbw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ntdnsdbu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3khnbeqax.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qpbadght.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ryyzwtie.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trkxuths.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fktycilt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkbvykne.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tmnywsen.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mbeiiihh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3slqgiifl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jsievuwg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fmifqies.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bulmomwq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rtkvyhzd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qbfdvrlm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llbhhhgs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uulvdoan.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bazlkmeg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbnpas.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nejdnknh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdhldvb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gopkbapu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wehubmdr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3onldgntw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kcrrmfmq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zsewitxm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kkdovhob.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3shqladgy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oqzoymwm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fufwfdak.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ayjxdxsb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3imsltype.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3djfrqund.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ycbvxekx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sxpgpyib.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oxpbfuea.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ztbbtrdp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3lqjqojta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zemslwjw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpmkmnty.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3sshrhocm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnouhqqw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3amcnjgul.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qtsetinw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lpfndwzd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rbhbxlql.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pivrvyyh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bbzoonqk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3emaiknhw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bwrtyxoz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkjfispu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3loqjpfit.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cnhzegoe.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kmmkrvap.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lpbyvknh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pukcropn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3davwmign.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvsopzsq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qjqytvhr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3popzepvc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wksnvgsn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxiakiln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzjygsgx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftbhouzy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3spyybsrl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3sreqwxkq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kllljyrp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3munfgelx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vuwkzixg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjcdisp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3geogwddd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbfncjcs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ovwzsihq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vekmehzv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yzmdytlg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sawafayg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3whwcwyip.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wuhnpcuv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uwhbqwuy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nbqhtbga.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uondbnxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wgfsyoba.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zkbvcfsq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3chzlyrmr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3umykhiix.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbifnhme.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ttqhhrew.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ntgsnwab.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hgxzpbwc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3klrbrjgl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hwmxzcsn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jdgvhqba.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqmpsecb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkfjjgjb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bdjdmscv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ofokhazc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ythjgqnf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzeyzxpx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxkmqqwx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nxtbjnpi.html


<!-- 参考信息 -->