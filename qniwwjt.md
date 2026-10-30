代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsjtqeewk.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/guxodesnn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gozumtems.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gbuzvwbix.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gvtisnjux.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzgmknara.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ghpgbhgvo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/ggvcczbuh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gitkrqezl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gwzocudve.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gtumbuzjx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/ghjpxgjdv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gnqlczvee.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/grkszbrct.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcnaugazp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/guxkmoden.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gewhoszrd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gasrgalsx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gqexcjyrf.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gdnymryrj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gfyqeftxd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gjbexaglm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/grsoqkyrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gfixjlebr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/grlouojcc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gddhbvdfu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gpxjfyqgm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gpqcyambz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gnvkcuuqh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gjoaxvxdk.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghmryfcrw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gohjihysk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvjiqocxy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/grjsqeidm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/glnuyfsaa.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxtdwlhri.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/glmbvwffv.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gomrjwnvg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/glgqbrqer.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/giphgumjo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glxwivtub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsclklzmy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gsyeaivdt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gamacempf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkungpcgw.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gejjedjha.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gugtdtbet.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gptikrkjs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/ghfjxuzkk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gthzczdih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gvfzwrezl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gqqrbcwjs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gdxsqchfv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gyuvfzpdu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gfbisjulr.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gxzgrnzcy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gmzhdurgl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gbnrrarzo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzaczbpkz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gmnatjvee.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gbmdngkiq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/guqnejauc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfcqdpitz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gilhlbibl.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/goybfqmgd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxdhjfcng.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glwjulaji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdtqlmcys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gfavqadpu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gclnfkxjw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gkygextve.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbttbqary.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gqqklqgsd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gjhvwgpmt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpyhwgeiy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggnorracm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwjesdfgp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsrlrxndu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/getwlcvji.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtylzaoxp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giyeabmlo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gciuccdzk.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gskjwwkat.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmqwnhqrt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/grqrqwznl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsbfkqvbe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gypvvgpfa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gsfodzkst.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gubevaehj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzwpuudqn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gisepnuuc.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gukpkdlaw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gxlrmlmlr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gcqlahsjl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gaxgxpvxt.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gugvpubbx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gdkxyqrzm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gdxiedovf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/giacknxkw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gxsekbzpu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaysekmmb.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/ghgkoeges.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guffucgvj.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gnuuruotn.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gzokuyoju.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gnmmvyzov.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvaurqmdw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gkplwjard.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/golrtamsg.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gbumerjfn.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsnumeccs.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gtcawnpsq.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjyuixtps.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gzqojqhzh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gkwxvqddm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gurarxnka.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqgambzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbwmiqyxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gqjisxiex.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gaxphpzqi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtvhkajmu.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/guzxjyfpr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkzzvtzql.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gphuqiedd.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gzdvdeasv.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gmwnqbwqc.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/ggjadsiks.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gsbmbxlfe.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/glmboubkq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/grbfajkfb.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gqnsghgvu.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gxltddibl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gyplbzlln.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/glzgelpcu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmzntartu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggnxhyavb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmyducjhv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/goykdkatl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gmptytgpu.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gtoezntzp.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/ggzmjcqdl.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjboeeted.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfatjyzqz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjxenvosw.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxylnpxll.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gdeehudrw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/guxbtzwvw.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gjrmuxyyr.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gmtjvcgwh.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gpofmxflj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsneqmcsy.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcqkmggin.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gtrkntecu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmlwjookc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gwmjevois.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/glrpgeoof.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gohnkrvom.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gfnhcsseb.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gvbaqdsnh.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gfmloznfb.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gwyfxbrxa.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gcurxdbcx.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/girnjsybn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqacrrydg.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gzehxrlay.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/ggksdkvsr.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/godfrpisb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gzixgusxk.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/geqdafnvo.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gclhqjnyp.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gawwkbltl.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gtehpxmtr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gixfpqrsk.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gbknbwlaj.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gyshxswfv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gdlqlimew.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gsobvhuwa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gilobjwht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gnbnjziys.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgwlliyq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/greevemdj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gtmqpaovx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gvnqwathy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gulktaqbf.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyahfbikk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gwnfaaele.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbvcfzzsx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gtzmoxowp.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gfacgqzyk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gcclntvvw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gjynvqoiu.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjqbjqjyy.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/glpwgkqgz.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/ggqhyfzcc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gpknsrvmy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkxyjtdzd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ggrywlpnc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/guvinjprf.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gowavahng.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnsznaeyd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gscskqsbt.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gyovkibbv.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gbdxbzpzc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glnyjnsxx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gfuzqxwgo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/giuxwiscw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/guxnlndsc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/goqjjrclv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvusyqrlp.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gyucsjjej.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gbzdctmtk.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gveyeheez.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gpkzybsml.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvwvmzddo.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/grfbxecvi.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcoevehvi.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glaqdsnqu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gmlhbnlkx.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gworoyhlc.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gjdoqbdsz.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gpsoefsqa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gybblfrkz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gdwlibhuc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gnnfoezpu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gwfedexpv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gkoluvnjh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gobgwwpnl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gzqevkyhb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gohhbamzk.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gzmkaebnr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gmypwnged.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gbdbgzjkm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gccurekyr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gtwwixqhy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gimyyfsah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gupsblged.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gouetgoef.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gkhibhawx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gwiqaxpjv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/ggzzyngvn.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gqoldivbo.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gtejqfldc.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ghqvlfftc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/grasdjxcu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gzbfgfbuw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/grxzhjmmq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwkaaudbw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghunfcqnb.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gwefxuqpn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdbaxlcel.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/goezfanch.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gyryiydav.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqluifofk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gxtejbsbe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grfubjzpc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gjzqalcbi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gythrtoax.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ghqztimoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gdqrdegzg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gaodzctvo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/ggfrxjkti.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/guodalxrj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnyirgdlp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbjtonpzc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gseuxmnlc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/glfgbjxrr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/glvnvwlmc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqmrerxop.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/giwdpvlev.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gqwfgeqtn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gonbshnae.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghppewfcx.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gfddrqcho.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/glltisapm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gkmftgybd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gxypesfbl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggycfrfpg.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gokalxmxe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gfczcjozy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gvkkxoqcm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/geqvuzsjv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpxzissay.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gkzfdhjch.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gfcpxukmu.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gksdplzqr.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gfluyybur.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gwoywwnev.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/guskxzzhf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gnwcptloc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/glfaexulu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/ghgeuyjxd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/grkbsffpt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gjyeoqyih.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gthtxofsi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/guevvfeyz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gjdfrjtxe.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/ggelqcdcd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/glbwqvmzf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gnzberlvx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gaccfsemh.sHtML


<!-- 参考信息 -->