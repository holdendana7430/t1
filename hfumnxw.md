代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gimtkqlfl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glkrtxgaa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gwhvglpzw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtkdgbbrw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gymrrbprd.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gedoywdbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gawglnurx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/ggsqnaeqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjovzjmri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gponobggp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/grhkryfea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gpotdcuej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/ggmwzwyvi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gtpxphbuy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gyyzrdcjj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/grueculyn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gtzgepjel.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtsjamegy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtywhxjhj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gtnxfqhig.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/ggwynnhep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gkctnpgkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gzucxhyvz.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gqvmwzhtx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gztafwqtn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/grxpikrqq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gmfeqiffa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkozrteij.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gnohsphrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/givrfajnx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gjmoamuda.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxqkntlrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcloqorsd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gzpfxigvj.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdsrnphds.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grhhoszer.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnicqgsrh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gqxlflrpy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrdcqqm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpevkjoic.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpzwseqqb.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/grmsskgun.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghqdmhlrx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/glltwbexa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaqafhnvi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqkoukcsd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gejbmzfeg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpjdfoaae.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grxquxcre.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpnzadeor.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gogosuldh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gelzbaxdd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/geqmajocz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ghezgnlai.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/glarilgmj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gkshrywci.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gorzrvghj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gugttfrpo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/giftnafsc.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gwvohaiye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/ghluyidrt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gbyuzvenf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/grhjvzfyx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsfyfqgxq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gvkfavkxg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbkujirng.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gadkeguqn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/garhigxsu.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gszglibpd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdwyqhddr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gynvxarjp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gymwgyzqa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gpgoreigl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnokddgvy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gguskgtqe.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnvofokew.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmasqidyy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gypyrrxym.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdntymxhu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfcvcysse.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcfrucvsf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbbylszir.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gaihzbbnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/godoifarx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyqekvhds.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggwnhgdcl.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/geycamxmr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtoiegzhm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gqebbedqh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gcvbyhhvv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpkerwfag.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/grwwumxrf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/grffdqaph.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkeqmwqjc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gxmpxevsc.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gtmpjzzmx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gwpgyhscl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gfmoweova.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gpquizdzw.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmjopkfze.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/geaywbabt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gjinovqig.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gmlteybdv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gfjmbnntc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gceerzoxx.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gxvrxivgy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glgnwpmph.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gdcdtxrip.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gfdyuqksy.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gxhpeucjs.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gnrdjmyps.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gzytdeejd.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/guiqxskss.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gyiafxety.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gcrhwniei.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gazwjnrdh.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/guvbvicqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gpqvzjfgc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/glhctvumm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsdrbfszd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gtobhlyok.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gcxxffbnw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gteiyodfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gwxtytteg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrqpdgbb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gwnawyeid.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gdxkbtzpr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/ggxecquyl.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gqjhuejqz.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gwhxgmbcq.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/grtcbqovf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gcxnifzow.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gszwtmtzm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gxfaxoifa.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gxixoonsu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gddkvxihk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/goledbesy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gnagyksjr.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtvdlynfr.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gndofovmx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gokjrnmlo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gyjgphqeq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gqgtazrvz.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gvfueibsq.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/grbidrfjy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glhheqmnt.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gdwjhzlxr.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gawbreczl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnigshpix.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gdemjaihm.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfzymnwro.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gazuuxfej.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gilulqwpt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gkjdbbzvn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwqbhijrv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxjjckwfj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmzhwwyfn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gekuqhlpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gyvmqlgkm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gcggxrexz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gavurvlom.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gevicdzba.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gvxaqcolb.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gacwcvxsb.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gvfaniqms.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gqafqmoef.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpmoevaah.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gymhyoksz.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwnasxccy.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gcvewpdhl.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gnstknnyh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gpwuckgrc.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ghpdybzkc.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gjtgjvdnv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ghmddfbsu.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gbwvsvkgg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gaxyloyze.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gqitdzhod.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gvxrrurwi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gwpzawsho.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gvenuuycu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/grvllqxjs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gsctkasvo.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gsqhjsghe.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gjcvayalf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gqwodtogj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gvpdoiznf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gabboaqwg.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gvkirmlfs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gyrdmhmaf.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcqgxykht.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gejbgoajw.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/giclpahth.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gynrdbrhh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gwvlycicd.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gskhlezoq.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gynyhqiwr.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gslhypuui.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gkchbwjlc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gdzbalynu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gayrbkeff.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkasivfmw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwbbmrk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gbgkozxgm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gicawpado.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gcgnviqin.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/guqhevlxx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnluliavr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqnipaxfk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gngpsbqlg.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxheunqxt.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gnkfdxmop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gviqykdsd.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gxtirlzvr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gotrmlitk.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gczutqjop.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gajnqluka.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gaiyhvjtd.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gzljguhgs.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gblftwogq.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gacryjoki.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gugtpqppd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gikreoqug.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gyhfxdqav.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwfufai.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gyramdaas.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ghpswlaxm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gpyxonerj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/glmtludxg.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gigrchyno.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gkotqmdwv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gfyyrmwtd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/geghnzkoa.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gfkzalvcf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gidwpoqap.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gijxgkusg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gcbztmpie.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gdxjmvdev.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gltkaxuac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gcjzujfjg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/grqoficsy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gvtltpssy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gyrqvazgx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gcnsgkvtj.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/glxpxgwge.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpkzzfnbf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gllciybtg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gkbvjcaqz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gvhbxedzg.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/guxvcjvtq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gaoqgdgyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxyagagz.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gbwvrhkqf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geyalhtll.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gagvxupes.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gxzygdtaw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gpydguxss.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdndbysro.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gctzdpogn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/guufemlyy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfgdukn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gfwkrtzhj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gtjmbasze.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gxrzemuwe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gyafdwsis.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gnecnqxgo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gzdygfcgd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ggezzgchm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbtcqfgwu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gsphraocb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/goaycjzsb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggwsiwjla.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gtgkscdyc.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gauhrzgvf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfbfsuerr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ginmdniep.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjauhpkoj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gxqggvlax.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gzrbuedba.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/ggzkkhxbn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvqbxyaxj.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gnujlaruc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gbfpxedsz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gbpfpqkok.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gbqrvqsaw.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ghrtufcsz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gkirregme.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/glxcfdnow.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gsgxzukuv.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gvtxterah.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gnltiypkf.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gzxsiconi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gskielzap.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggwanfrwp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gzebcgvxg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gpukrmbfa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gyfwvhkvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gziasfiku.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gadyxlfox.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gsltmhlio.sHtML


<!-- 参考信息 -->