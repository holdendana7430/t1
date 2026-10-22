代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wluedmzs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wwqgpenx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kolvmdzg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2spifsjkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ytelgmaa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dfoopwtf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2xcobmyhm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfgwlssj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdabooyw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nijuvraw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hhbkollv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2iqnbnkwz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekrgtgfw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yhuzvhiz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xsyusjda.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ypzhovcn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqnfdkd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2buldofkw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yrotlruk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uxyhhgvs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2paygtxrs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dscfujzk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iadhomtw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sholjwnl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2iqpghcoc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mlelcsxo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dvakxzpp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sdmzjcuu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ciccaqtc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bjblxsbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jabiuonn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mdbuwajh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dnuxdzzs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kiwxkzxc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ibopicdx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hjbiapzk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nbjwpkij.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tccpdhlb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umrvrakw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfddlimi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eufnfnsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tsroxqor.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vmnegwxf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxlooqfi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frcczgha.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jbctvgqw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfnnfddx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ohenrwzj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtstcfmi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpyuihmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lhogktak.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyswissy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlrprwoh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awanngtu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wjmusjdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iqtefrvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hmvtpznb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2caocilfw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gkvlahhb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ctnuluan.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mnibcwqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qtfmsnfu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zocazqfx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aokqfzsy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vondhndb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rqctcfjk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2getagrpw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mosvjofv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ddzagmcb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qzyyitgv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2unarwexk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2olyibjrt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgayun.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmwsvote.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2adeokqic.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rjcukpki.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vxsvwlvk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mufurrgt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uotcgzip.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swyzhqrt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zsriklvv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xofgmvjc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vofvolcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2whmqqwjw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqqibwnf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxpqsviw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kdaxrndl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abqtspnv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjczezyy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxoaekkz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwuyzyyq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldkezumv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nxzgazgz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zskhfiey.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfgrhhvv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2axlsjtmn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kezkagop.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrguhbfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2evygivak.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cbfnhuqc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hszqaxdl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vhshgkiy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eduhpchr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ppqxxwbe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lakpdcvo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2eexihfye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mfjvneva.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dzrlxuaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pggseied.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2iuxwwtdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2curvkllc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gkjrduen.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gfrtmqeg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mwtcktqz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jymuohol.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kphydhdo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocemvosm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qvbjsoae.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pywmczlo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aspycbcu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tmxrhalh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ydrvaxzl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jvqofyei.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrzdshln.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eedllykz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2prxikvfo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2locajywj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lnqprwhe.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dwxkcgpl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xtrohzmn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pwjhxuup.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xiptgudm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2noqstqcs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ztexjezv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2knjvilar.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ukekuqhr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wzgewjwx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2otjhxcjd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ceccgkah.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gdwpmklr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzmvkmj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcsovpch.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orscodsy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwfpbuyy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2perdcmvq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2blxmxckh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2svtnwnsz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2alllyext.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ymurcuio.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifjoujqe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sighselm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ondfyyah.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2asfhogyk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kjftinli.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2rdaxxkrs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckwpjwtl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qjqdqqou.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vnvgwqof.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bljujwnm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2noxoegzx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbbbvtex.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tkaedake.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2omehzwnu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yncntbpd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ovvycsus.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gdudirzi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2khqtiwlq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kakdwlnh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dgrtmfso.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wxdxtipt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2inlpeyrp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hkjvvjje.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2woewuhcy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wmzcuier.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nkawnatc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zyplqjbl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihonyyws.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vykqvntk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jppcmvuq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2meppcrtp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tbymjean.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zymzkutx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kmjkexhc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nemroiak.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fegnvhnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcaqrsso.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hoyggdlr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2igiyqojk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxsblehd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2utwocsxr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wrfihgqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fygkbbds.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jddupuib.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tmujmbrk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vegonfzv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fmxmxpiy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2flbbgcuy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jjhrqvia.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rawpujey.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kszgnbuu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pwdredza.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2udsrkbrb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ajefaucf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gpepukbn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ulivpgce.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdvgqlqa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hvysfpbu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kbapksfe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fztkctxb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdftjsmk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2empnhhko.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fuxijbst.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tkuvosbh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oeqxpgpl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aerlypki.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pmptvfjt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2azseclcx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggcvmgao.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fpqhkhuv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hhlfzhjt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ryxeqapb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mvgcqxii.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qzshfptz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lzigapfj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xtxeeeuy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2abhlyeyz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ltqyprrb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2drddykpa.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2adnpmxca.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fyrzfzgr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ltzivjnq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iwnttdsj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vayjkxmp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iffcplnc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ttwgxfsb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2shdllmvd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2eyhbqryh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mqsdwnew.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iflglrov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2sxztihrp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ayduegaj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sjtabzzg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bkvvrizn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2oixhjwph.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iyhrdisr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ubvsknsd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mhwmlwea.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lfzeqnjl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dtnnyxtg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vtdfcell.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcofohnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2olwkyxrl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hqvfppib.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fjsgeseg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2snhojhvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hulsrqkn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gegnirgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aextxelf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xyasapxu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uvumdsgm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2exdirbpq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yavyznej.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhrekhe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dklxcltz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dmmwlrpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cysidceg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pszhckom.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kpkkjrjb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kyiyvwmh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2njgzxhzg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hmmrvatm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aipnkxcq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edjwzmpr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2oyzdilty.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2oioduipy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rdjtmfag.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hqnwvepe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2djmbbxpo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2azkohvmw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qajksotr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ioeoczlj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2srxxvjja.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ttolcweb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qoegvtml.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tmgtmlmt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nuhegjsv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yzfprpsp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vumiupog.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ytszhqcj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xozccugj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uiahbspk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2baratvrc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzmcnswr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyqiydcz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2szxfksju.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pmfhchrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxldsrar.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxfeuprq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdjcklul.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwrimwaw.html


<!-- 参考信息 -->