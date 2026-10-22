代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nbkbyarc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpzlxjhd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qfixqfju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qunmjwkn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dksijuah.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eiapeyrv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2roldjymp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gtcdqvko.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xcgkpmkw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2odnhjwgz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mfqozycn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrvwrsgv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hwydemfo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vwphwsoe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2csbvumld.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2aibmaxor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtqxylgt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnkzxbbm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wyxwfyzv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mtbnfnbf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pzezyzxw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2phaglmcn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tquqfkyj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gdclward.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cgcygkbk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2otoqtffl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fnizrhce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2atifwfei.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mzvndvas.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ehudmzqp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ezvdmwlk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfomcoon.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xjfxabxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fzoxygoj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rolsovjt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rkepfomn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xrvnvzlz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nzzgbydy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjyjwbac.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qlvlbzkx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bdjuuupp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dxnbraek.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ogpvrymk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfdplgrf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoyzdimt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2egosssvp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hlseijdu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osbcrbjl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uufbbgbl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2imbteuxf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrtvusty.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhuiqucr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvwywkbu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lttiemha.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eoijkbeo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnliyemt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kafxjmrh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iijgaasa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2cphbbafw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rrkrvvyd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgguuvab.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dtdrfdge.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nqxeuxzh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fwanskjx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gweksxww.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2twdupcrp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pygauuko.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uambsysq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ndowjcix.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2namftcvn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vsjlufmd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gwgcwetb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tmizsswm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gxvnaamw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sikpxyxn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2txdsncax.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gzzycxij.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqldocxg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tpyqvprq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gwybedua.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vnvsccxx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cemwdruh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2aivkdlcs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmlmcyta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2meveoxml.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rwfifzeq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckjyombn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtmtbqra.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tefdmtqb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaampbej.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zdfinyij.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifqdypis.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzromtgj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkzpmypy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2abxkthlr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvzytnlm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfpcikgo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uenxtozy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhqkslrs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jnpcnpnf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lfifdstl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bttconvj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rmihrelc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dnpbvrph.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ukgdlxwr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hznxyicp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vefwazfq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lkqinstl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iwwxnijm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bzqdcyuk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hjraoedu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mzpzswfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzbusryb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2osknubnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruywidtj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rggkkyee.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xypulfjl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvnjitqv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fohxwmxq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tyfqaykp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ihxmscjp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tpnzrdkc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xzjegdhb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbayrgot.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwhhdvto.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2glwyofhs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2drybnrug.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2teqcungt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqqfbabz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqvfpfdj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vncdroyw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ombbnvdk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2luqnflsk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mmgifmrb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qxfddxbj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ebdvtphu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ouvfspae.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2msfskgnv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2junefxjs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iojxhfrv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hdnfycnm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2durnxxgf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2suoobyuy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zumxhkvu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ainjbqnq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrmzjkvp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nhlcrjfe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwlenljq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tsdvagju.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2snzflurn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eifgnquj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vfjxfcpy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ponpmvls.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fgxfwtkq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gywzndpk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxeafdoa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcdjmtcf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sofjqpzc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gnjgtygf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxtowuiq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ngwgrdfb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2arhtfwtq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2llrckydp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oqgmmfju.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojtkexcd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcedgdhh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wnilrrky.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mhoirnqk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mqrzedcr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2feizvwcz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2huwbxicw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuylpmzz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ifskaock.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rmqhshlm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2myeplrnw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gbfbnfps.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nefdysau.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mulygylg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ejnkxvod.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dyzshrtu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cdkeydyo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vyyywiqw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fhorllsa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2opwgscve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dygxhdaq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uxhknlus.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cwqjhpjg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mjqpkikh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2renlxswb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2odhcvgmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zwnutyap.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ywomqtco.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sgykkgrw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tqobpsgf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcgdnsec.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhipsvhl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2holyvzsn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2algqnoqc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qqytjqzv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hxjvkvyy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ifayxhec.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qlavwbex.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vcqsbbir.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iyjritbq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zfguptyy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2okdyuapu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qomphjmw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eempbwua.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2splegqza.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggxictle.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pedwtxlx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2flkklxno.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xtrqcnpa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2luottutd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yfrbbbts.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tadjnxoj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knzmikmb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnqydsri.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eypwuxqo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efaxpmss.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cghvmcci.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2thmvobjz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gargqzyp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2edxdozaq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rkobvhff.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xorivqan.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ewsabxwt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vhhqpajc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xlrcomxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kjwdbynw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zucnnbep.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bmvqcixu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gllabfts.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bgqbyzmn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qeasptim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2usrvpcii.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gijkhurq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfofvjrk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2slhoccqj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mmplqdsz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uitlimki.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rdhnmdct.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2sddtjisp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzjuuncb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tylimcto.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2onuymkpm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mwwkpdsc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2llafiqap.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dghepvan.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbklex.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2aiezozle.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xmpfukpq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tnioafkg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvultlkg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lozjxzdr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nndtlueb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2pvgptfav.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xgsezkae.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rftucler.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufunqrrg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjnwzajx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhkqgoxu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gfpvldqg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ufswvuhz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gyxoxdse.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2trvozosw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxsheicy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2iiyannlh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wsfcgont.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lphayxhg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwcqfev.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ytputgis.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oqjodttb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypxgwagc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jxuphjzb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swfwiyvy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fsgaesgk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zywqwodk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ljoplasd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lklmyifv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2azkryhas.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mxdvyxwo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2drhddxrb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2werthbdp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nkizlshk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bjqbjjlb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2iaayizek.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ejkofocl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oyeidtzc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ailzznrh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lcwjnwzf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vervtnih.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wpcxfawf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdqryncz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykywsziy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvzeigy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2uraxrfxw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mgqawrfq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfjhadnh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sfbldhud.html


<!-- 参考信息 -->