代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggdehvzta.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkzqppmpj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gbnlifkhr.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdgmxgpyf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqumrrmme.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gjwyziawq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gzivxdqeu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gkhihanaz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gxerqllzt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggwpvtskr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/goukagppr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gscidpfny.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/glhvosjdc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gbsvryorw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gitgqmqfz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/glbjdurld.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzzrbwkqo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/goztycacz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjmxvikyv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gpmtzsnxs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gpsveurvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gneiyvdyg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gnlzzougo.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gxgzklijp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gmpazfkfr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gtudgbhnk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdvjkhwzs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gihzqfqos.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gqokvespy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvkjiupko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/glnkxcevx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gaiqxzweh.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gmwsvbjfd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gwqtfjqki.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gelbgambl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsqjhidah.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giyfqsihw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gniihabfq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gsuwnqyrs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsonzbeib.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grxuwulkv.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gyakmendi.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbdfarkbn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gejlrniag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggbvjapui.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxjomflcf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzfnhcdzy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gavocnivs.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gotpzvcoi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfersnrqj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gfcvdyhxd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqhvepfbz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkaapfauw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/goyzngrea.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ggjcdzamx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gjatxtpcr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gbqppgifb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gfaveemuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/guyvpwzmz.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/glrfijncz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/grqbohprt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gcwitikiq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/grtozpnjx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/golrjbfvc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gdskmxuma.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gsggefbkj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghnnwclta.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/giwqqeins.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gzriygail.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfyjsests.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpovofakk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gexjotgas.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gzwmmasno.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtsnzanau.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gxtgjivab.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkllplava.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/ghbahclnz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/guoqjpjed.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grixdfomu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gnfziwjwj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giodnxpdd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdjsaiqlt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gkntqfnco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwjdjthaz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glbmosvhf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gndurjooa.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gprgrmjwh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gurfxitvb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/ggrcwidgt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjpvuvsfs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcgbkaido.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfjxbrfvx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqoujaumq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjvehaxgs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gpggeyaeo.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gjnvinmgs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gqgcprxor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gmmcttgrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gowrmauwb.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gozjmkooj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/glpezolda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/giyxyzfcb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gbqoiucib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/glkwecgvf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbyikpawv.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/ghvvbemre.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guzyhobhv.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gufjtzvdf.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/glmkfgnis.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghfubwuku.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwumpbltm.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gtffohpwm.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gsjwyxjqh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gouytlthz.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gzsjmeepo.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/glpjnioar.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gexmilsvg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gfrglprsd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gyebdhhoe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gotgnvggl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gslsisepl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gdylxpypi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gdlivkwwg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gdywmmkea.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwfhnpoxy.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gqyybkbnv.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gplbnpial.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gvigwgowu.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gaogphqha.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gfqewixkq.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gwnvocydc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gquzuazbx.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gwirgdncl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ghuhrevgo.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gturnsvuw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gcorhcoel.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcsljpqhf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsopxhbmy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzzrjxpdy.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gfhkabkpy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/goptojkxs.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/ggdnnnsdv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gueuysext.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gpplkrsyx.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbrsgmdgj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gapsllxjs.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/girnhtdjt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gekrrlzce.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqsfanygj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gxxqteokg.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/giogpkopk.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/giqjhaajo.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gfnffxuzl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gmkydpvoe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsgdtponb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gthrzgyzv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmlejpeww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gygcxaicl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/ggawakttl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/grapxfyoh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/ginnmcvis.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/godmspksw.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gafxdqbrv.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/guamavucl.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gstpwxcmv.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ghoakzcwp.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpvzchhoj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gbxqgbleh.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqlhoprxk.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfvtepjpy.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gzyjukxjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gksgfxpbb.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gbvxuziao.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gtshsknrq.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gglbhvvmh.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gthfqtjjj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/galijwetv.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gmsftebfv.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gwpvtljjc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gvmdyxhcs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gifonadgo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gqctizvhy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gyyntpatg.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/geyaohmtv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gkrskodqa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gsknkgnbt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gqfngwpps.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gnwfnijwk.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gnlyobhyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/getmrxlox.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzhupvido.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/glxbjkqui.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gznqwixeb.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/glmgftvbj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gzeiewzmh.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gwzgwxtqj.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/geftldxgs.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gfljjdyag.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gwkajhzgo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ggozioqhu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxhmpvmv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsbckukbe.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdznbtxvz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gcxmztfpz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gxafhgqen.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gljcducua.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gzhuzopxz.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gboqfnzay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmaaiazvm.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzxydyrsw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/guanmevng.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gwircuhoy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grdqqvwdm.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gwbjodxkl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gzqfxpeko.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gyubmfupi.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gbhmfnrsw.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gragyusdm.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gejrwdxqi.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfzduhmsz.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gefbacvju.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gvuagwaqi.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gtbwzvxuf.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gxkjpzxcl.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gabrironm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gdjemopjh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gmegeiuke.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gddxdmrit.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gvstqfggv.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gzmxzcvpm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gwgcknroq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/ghyquxhvp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gxjpojtee.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gvvpnxxlj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/groqcsftw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnodxavc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/ghavmxqiv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gnophvqvw.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gqhbqdbqs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gpyapansw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gzcctdzag.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gtnvrngyg.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gednviapu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gtbwnbzpb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gvniuahxk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/glknrptgi.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gcnkmjumf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/geatoyyfq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnedkvwnu.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gbjacaemd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gkdvrytcj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gshmmhpiy.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gjbzxfgzi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpnwrcoyw.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gujvttgct.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gdpgkspse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gsiwslwhz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gehqdefgz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ghqhlmvcw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gupzofwur.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gjhbeetld.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/geytklqmu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gnxisliyk.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/glvuehdsh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxujylkdv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/goihparsx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glvcmnntl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghkdtyhqq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/grtgcqgby.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/galtaglmi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gpdmczqnu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/giaoohkuj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gmcimxbzr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gkajsioqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gnlzqqphx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gidagevaj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdsfmhwlw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guvuzcpqj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gmgysbpch.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gkjtymieq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzgpngfcx.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gfeaxqmqo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gsihkkrsm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gwqgyadjb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gocurhodn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gicdrppsx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gowjbpimq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gxjrupvqf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/ghgsgvwdn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/glcnxaqcd.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gswyxiyjk.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gsxnnwzmw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gvisahivf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gnmsyujoj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gmymohdyh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gnjfvckrv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gssxdueiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/glvvavlni.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gutyzyoxj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gddwrbipv.sHtML


<!-- 参考信息 -->