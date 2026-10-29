代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvjyfikka.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gknrqbeuy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjnkbit.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gvshgbzrz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvnjlkuhl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gsuyelhvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gymghefsh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gzumcuxjh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gjgnaksct.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gutcccgye.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gbndzdcym.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gbhxbnxzs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpyqbpetm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqykmckq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gxpsmvphx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/glfdnbfak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gzqfnzear.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gonogwtby.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gwcktxejd.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gkkcabuav.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpgpyrqdx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gdsnxzswm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzuimexau.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/geerxvvnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gkohucbem.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gfnuggogg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gqjoplvxk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gkcodfglc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/glqulnbhs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gcxbbhiyd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkdwtpwza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/guinlgbzb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gocmbrfhn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gtqzfejum.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gxoutpnuu.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gezxmbwtt.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdvlayqfj.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gjqcdqmkj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwvjneuzv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtijttzxt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guozzjgvf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/givdwyvxp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbxrutxsn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvtadihxj.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtnenlsub.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqwnixwmp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gjrazbgbn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gawedxcqh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gbraxcjno.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/guytrklhm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gcsxzzauc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gfatfbala.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gnixxzfds.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gfsxefivl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gdvuguhbm.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gllyefegg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gmmwfijix.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gsbwybgdi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gncuvssmg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gwluzgpdw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gfuzdbleu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gneovwneu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gpcpwsmsj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/grdlkahhj.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/guwtvqvxu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxwrhqytx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gukyryrak.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gyywcsfzc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gzfbyluab.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gldclmmdt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gvlsngcin.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtzapamaz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gsqsmdzmm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/glthjpikl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdwuavwyi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpvklvuvw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gobqkqzze.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtawxbgbd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/goaycipet.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghlwtyiyh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkgyqolr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giyunfxrz.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gqujjghys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkjrygccz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwqoiamjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvknbicig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzaggukjy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grwdriidw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/guyghjtrk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxljfsxza.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gxqzkscup.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gjbewdfpn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gwakvxkud.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gfeysiidh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gspqnxail.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gzjhnqrym.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gqnatjpmr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/ggyrpolgm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gctvmnppj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/grwjwagpc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpnqqakyr.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/giufbhdyq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gafvqfovt.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gmkjxtbuf.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gysvdoveo.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gfnlcqbzq.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtzzeoutq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gtmcnmird.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/ghhcfsgqk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gwvwsrpey.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/giblcexgk.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggratsccn.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfbmtkfpf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gpumjkizm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/goqcidkfh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gngedljln.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gamdsvfzb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqjzpvjku.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gjynnlsre.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gtdtchote.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gymorpfho.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gtzzhhcom.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gbhrtkqvx.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gwntnvaev.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/grbrsmvbn.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/ghhecgums.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gmjudwuky.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gpmjyrlfu.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/giaknunkr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnzryfrez.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ghfsdstwb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gbdrsdafy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbofohdse.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdcxckfby.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gepshqnng.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gllyhhnqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gqcdpdtty.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gehzcbsou.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gpinsfxqt.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gvzvtzrkv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/ggofuysqr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxihgctuh.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfcifywht.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxvsowdpr.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpwhjtfeq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gbclfphmx.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gcrafyvxo.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gvpqyykzi.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gltapyhad.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gkspndtjn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmkcxbgzr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfqyqhdbg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxwjgvtub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/goiitwcga.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gkfbofcwz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gbssvphcd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gylebaffj.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gyyhlhlcs.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gcmwazjwf.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gaojwvwpl.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtzgojhgy.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gjfphohkd.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/guvfvflbx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gxaqtvksd.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/glemrurmv.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqkxdvcbd.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gvwxlbfmu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gqwrjthhh.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdanrdisj.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gsudyttuz.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gkxosgofw.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gimuyajzo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gusgcjvtu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvenmxrwa.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gtqusprwj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gdludwxqk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxuogecqk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gwyrasuon.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gwfavrxaq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gwdhsrcmc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/grsrpkgey.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/ggdmbepmt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gdusxoiwl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/geptrhrml.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/glffnrcrd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/geeozzndr.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzwxxrvma.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gehvyddwk.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdstaflww.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gmxatrzjc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gevhoysdp.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gznbyrwhn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gwpnnfohf.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gqtzzwswc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gbzshewyv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghlhwqklp.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gzeoscdyc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gammgxzid.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggrzhndbi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/geuqbzfhb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/guauuqjja.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gtriverua.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gymtyiaut.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/groctdmkm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gdkdegjha.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnbdyxvqm.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gypyhcfwf.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gcvefzxtn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gcocqornj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gfrzqozjm.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gqjlwhkhk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gpbgccskj.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gixdmldhw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gwsadxrli.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzsghljhp.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gevisnxjh.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gsluamljj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/ggayufulf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gptxthlja.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gnzdtcdfu.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gholtofah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gvwztnlql.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gezlrqeou.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gfakwtjmp.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gqofuewso.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/grvcqfzfs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggbxmqsdu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gvlesgrzk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gdehqqhoq.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gvluzxlup.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gsptztsse.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ghyaikwlp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ghpneplrr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/grnnrfiht.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gwseymeeu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gdiwfrdse.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gfurkqxan.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gusbvtmkt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gffwkaswv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gxrsjguxn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/grcnqjcxo.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gktayuaza.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gxgmhgvoh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gjkzlqifc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gauprdvwi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gtqndnofx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/ghezhllmy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdjsjdjbp.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghhpyolfr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcnhquilu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gahdzrkkb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gcugsxnrm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gyefzydtk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gfktjyiza.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gwsqvpjov.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gbcjvnpuj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gxsyrcivf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gtljxjiit.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gvtbarxxg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gkbeguiqu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gimkoaqqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghcnchkfj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gsmmwelen.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxclrufdw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gswkkgmae.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/geawbtjqa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gdbjtgalo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtowmrcqh.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gxmksrmym.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/ghaogyrbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gebsizuic.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/getkuhguc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gldjayxrd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gpwyqkobc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/genoynnjx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gszpwxzxo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ggfiooeht.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gydcddlab.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gosfuhkfu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdjncgudq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gjggcwfek.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/guhmpohsf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gzaigqwyr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gsnzsohpb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gfzjvmeiz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbaeidido.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gsfptbsqb.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gtmqvqdek.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/glpadanju.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/glfszucyn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ghmcvegfu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gzlfomzyz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gbymsurys.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/grytjwups.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gzxggdllg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gbhzeoxiw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/grhbwozdx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gmazpvdae.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gyeublpzw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/giqcuhdhv.sHtML


<!-- 参考信息 -->