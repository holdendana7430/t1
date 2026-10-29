代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gwffrwhch.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/geqlpmioc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/glvjccint.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gfjlmuwnm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/garvxtoxr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gjifzwnar.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gzrqvzfvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gghagdcqn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gfxmydzsp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gjlwaggdb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbwdflbsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/ggyedlskw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gfpdrhgzj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/grkraglbn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gcdbbyzbt.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gqnrucpbq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggukxuvdt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gomlqepyv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gngmkpfgy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gycamfbnu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gpuovjkzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/glumvieir.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gmzctqrgy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gaztygblq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gtferjdzj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gophyeibc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpsritxyr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmvktxvbo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxvkrzsus.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxthxhzhy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gydrfcxfm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjpczkrdz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcfiladtg.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/grgaponky.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghupdgybm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtddkhoxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gskiexhzl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giwifqvna.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghungrgpi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfqxuqnnb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwiqylwhm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gusicahlg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gsvwxypxg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gduesvpjx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/ggjoznmsk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gblzpnuyo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gzlzzogpd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gnydqxwcc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gmkhyugqo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gbajdnins.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/grwzbzdys.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/ggnqxvhrg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gxbmhyxmw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gksivoqob.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdnucxfxa.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/geybknvuh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gqgqkiint.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gaekelfjj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/grzmnzsmz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/grqnlzoze.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gusvsfymk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gduqdsfiq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gatglljut.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gkaqjmeld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/grarpjytn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxxywudjl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gyrvcxpfu.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfgtspzqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/ghlcphpya.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/ggnpgmxjf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdkepyieb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxggnooki.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/govzpdxbj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmdthhcys.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gngbsloib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/getihkivj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gzyxcdclx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjtulhnjy.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gcirpratc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gcmbycmxy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/grbjpissq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyrxuttre.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gynsuhfdy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/geivudfxc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/guraarcvj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gtmlytitl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gupqgjgyo.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gxxaxelbo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/glfbmlzuj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gsacqursc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gfavkkana.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gddhoujgc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gyjzadshx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gamxbbmss.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gcrolhuop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gfqdwpwse.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gybrmxuci.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ghhvnnkie.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyxjcphgx.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/grrxquyxw.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gjiepbmae.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvmchncow.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gkftcjfiv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gdkqyotlh.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gvfnhzzzs.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gmfsgsqzz.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gzrzaabqq.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gfelgalxg.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gxjxhchnp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/ggbdrkggm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/ghgkrzqjr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcvxlqfro.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/givdhbqno.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdavygtvq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gbzpbjidn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gssnhxkhs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpulebdnn.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gzqjrfawi.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gpqozonqj.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/grwvizanz.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfhvxtseo.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gafmisane.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/glhjmexik.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/grqkgtkhh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gpuhfggvl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gejikllpd.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gtquwdxdx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gchksyqtl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gxkrwzvkg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyqwuhhvq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdzwedaxy.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gssmfdgjv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gppeclekn.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gyujejhju.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gyqbdivlp.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gqnbbhfit.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/ggrkrhuad.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gefbryfbh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbmlmfpgk.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmsvmuexo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkpkknmiw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gaefthgok.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gbtqievtq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/garxmeqvf.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gckmylbyb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/ghrdrgdbt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfznktgbc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjbuwupqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gumcrysnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprwmsslw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gbygbxdaj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gbcfngxuu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gkukerfel.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gdigmgypg.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gferpgjex.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gjbgglrmz.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gvircgbqd.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcydzkawp.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gpcufqkwb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gbllmysir.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gvznizngf.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwirkifbd.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gzkbpteec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/glukdqqfq.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gitszmprm.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjnwrppnp.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gasnaidrm.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gmhwiwvzo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gnpqlsjcf.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gppuwrcan.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gtnzncyeg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/guwfaikja.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gwxhckqpl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjyvfowfh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gjmspotcm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gbsiluebm.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/geuzveogh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gszkkflsf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxrohpoic.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gddzcaolh.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gcqdizenr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gblggnggq.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gttmcnwwr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gpoiuojic.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gonrhzhze.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gyxmlsvkv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gzmptvvdk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghjprukys.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ghdgiawlg.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gneyssrhz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gslkdgdsj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gqtybnidk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gnnekjumt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gggirnnsf.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmdlnlgbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gptjnwgkg.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gvumzingx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ghjbzqerh.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/geqyeqxsz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gyhyhkgnq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gidxuyahs.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grwcfxsmm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvczcmrke.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gskqknrym.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gnlvomzjj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gcknyvthw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gdfwdbeub.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gclopbniv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/ghhcmzjzj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gvdxttvfm.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gshhiipmk.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrflkje.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gnswkhbzn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gjuwjymwv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ggivpwjsw.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gyuzxulfh.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gnsokhhja.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gtpjrfgdf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/grmsvpkbr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gzqxqppvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gnolxolit.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/godkpsati.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gkbhwhqdo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gwwbjylau.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gwqnqpysr.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gdsynlchl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gkspzdhlb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gpblxitab.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gnaaknqct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/glduyxcts.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gprmaoxkv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/ghihihyto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/geoayrcso.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gvcjxvwpv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gnemumvig.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gkxinuslx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/grqtxpekj.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gicnnfuxi.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaevjdzrq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gmjlumrvp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gkgrdlqgo.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/glbmkycyj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/glnihsnpw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghxxfeqi.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gevwxoiuk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjyzgouze.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gckcgkdob.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gwjrilldd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gtglbwbnq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gddnexdgo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gydrkwynp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gzbzsqqri.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gtazbrkie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/goxzhwrjq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gicwiqlwa.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/getoaqjts.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgqopju.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdtrufltr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbkplzlnh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gckzyfpxr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggopthumr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/guofuebni.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gmhdudwsj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkgaldcsc.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gmobdhytp.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gmsfzhdrq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvkbydkko.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmudqjzkb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gomklfdvt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/glkvcfudl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gvsyrzehk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gzywgehxn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gzhkzclrz.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/groqlxoen.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gwtolnxve.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gnpxaoczy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gpsyvuehe.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gajccrbep.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/grgiuegzx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gkbbghqsc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gatyjnpgs.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/glznxqmcu.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gspzkpgwp.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gvbtngpip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gztiymlex.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdaglsead.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gscuprlih.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grlcncrua.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gocmlnmbr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/giwsnphsp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gnzzxdybn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gynbygihs.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gjgzylufc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ggidfefqn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gvhwlnraz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gmylnkthn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/grrfvucso.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/glrmnwgly.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/guoezxmmn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gzelikkwn.sHtML


<!-- 参考信息 -->