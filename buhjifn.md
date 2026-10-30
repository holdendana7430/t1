代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gomwzsdxc.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gqijlalko.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gluclxbue.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gvmtzdany.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gwtmohdni.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gtqyjupik.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcqjkhapd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gdwyhdztw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gyupobobe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/ggjwmwgav.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gninetkor.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ggjepeaxr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ggwkqptfi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gaqxrdlgb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gglevnvto.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gnvddjufr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gmzerlfcp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gxlcqpwni.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzdieakwf.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gcpfjcldw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjhiiiovj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gmkugsrmk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gzbynadph.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gxokjchta.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/glxavwhgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfstfvraa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gqghgonxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gmjssvcmb.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gupgcclfv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/grjpqeqwj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpmggxkzw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzhkgmqkw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gouotidbr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/genxgqghd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gomtqbuvh.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghmohhddx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzfzfzxqg.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gmxckzuov.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtwotnulk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gfygmpbix.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqiqhmszq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gacwwyobq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghktylscf.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giozgmozv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqnaajlbl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvesugbfl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gxzhgqkbp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gnubxoarr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gydvgdmvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gfhxzjfcc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gzyppszib.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/glmqlrwsj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/galpuadwu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gpyptzlgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/ghxkglzus.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gpxwubnmz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/guyekrxyx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gtdkijxki.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gnqbrndpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gjqkknsgs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gdpnzwapw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gxsedbitx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/grzsbkaqt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gqgumjguv.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ghnzytgij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gysgcxbtb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzmsmcnmr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwtztlqdy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/grmxplpwe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glbrabfim.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gvexzthxx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkvrxfqki.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gtlzoozre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gprijwskf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gayrhviwh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjcxkxqdj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gclklhvzz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsltbljyp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/guubdlipv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsyplmwfx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gepbusflh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmrupbxzx.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/giyujlboy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtimbslxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/ggzppyevg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gybcfwjjk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gskboiuug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gjvzprbbk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gvslxlfjv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvvmektdd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gvizvwxux.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gkipfruaa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gcvthfwca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gmiegdowt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/getgkmdrh.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzlzlifpx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gjsptoqxy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gbxwrqmxo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gvdeylrar.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gtgphbfba.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghgxqiiqp.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gvvcqnwex.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkxudfqss.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbijtprjs.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gcdcmjwmw.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gfgwpestc.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjvlrlhxc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/guvgyxqbm.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gnitphbtm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gevvpetsn.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gzalsucbv.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gbqwyrbvh.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gxmbzlpbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gjskmukks.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gytwqbmgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gemllxfxo.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gtmqshsff.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvucgegkh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gnuoudqbs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghbyurkhd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gydlmyaha.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/goclflsvk.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gydyqbsjb.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gsieqpyjn.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gurbdxgrl.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gsjxwbpdo.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gorploajh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gtrtrzpip.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyteprepq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gdgdakiba.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gcdrkeltj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gbovhjqza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ghapzldvt.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gemgmqudi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gkbhglksg.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghmgwruwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gkdkcvfaj.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gsgjrxaub.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gtxjjedfu.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gcswvqaqn.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gmfooqpvo.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gczsqrsyk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glmlohtxt.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnxivpded.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbwbusnuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gfhjgwlmo.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gmmfiparc.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gjcugsyjk.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gdmfrunpq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gglaurfna.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gasdczwcb.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwjzcafnl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsucmjmpq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gszkdzvaf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gndwutmrg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxtfsad.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gqisgkoes.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gfbzhkxrz.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ghgluwxbv.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ganwrmspr.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gdmunaxyi.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gybehlxnp.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/guupydrcv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gdaznlkdq.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gzjzddknc.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gqqyaydlm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gdnmyxsxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gzrwxomzh.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/guxaienva.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/glitibluw.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gihqeqrkj.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/glkinjacw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/goryagphu.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gbmyqmgph.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxhqbdpob.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gphbjekpt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gzqqxfgjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gdkeraaez.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gymmxouar.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/grccpjvrc.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/glopwjefj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gijmdlblr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/giexqtmwd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gxzzvwqkk.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gujgpival.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/guunlwzcq.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gcuupfyhg.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gglirmiwb.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzkvvuufc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gcqmgxbrd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gkdxehxir.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gwdioxwbz.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gxsipdtfm.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/graamfgju.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gljosjplf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gudpvzaya.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpofrefl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtzijyysv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggnxbszyq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grvlxblkq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gvosgjcug.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gphzcywcp.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gvwvmenyg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/godlbilvk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/goqlrhwps.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/glevtwncn.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbrbiizzg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gkokwivli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gcfkivuxm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gxsztjibe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gimhfarcv.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gdlbvvcdo.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gxqnonqon.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gucuvyxmu.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grbpwneju.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gnoehuipu.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghobaxpgm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gfxaxtkdq.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gwrotfxgb.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gnplkpogp.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gzxjjdyrg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gtktfzmiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/guxrutust.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/guahtamsi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gpjwpyiyj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gijjscrhu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/grtkafmef.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/ggwbkingi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gqadxttit.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gwcrgeoan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gmlmzgfum.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gqolaiamo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gvfkapzqv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvluzmsbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gsqunfiof.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gcunsjcuk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gbqekzlvj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/geyksujuh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gqikywemj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gvylmguhq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gpziepwuv.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqciyfjkw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gmbljoyek.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/guwqzripk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gmeaxyzij.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gklldjcwd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gmebzrduc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjprdwcpz.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gxnnrtbat.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmqklblyy.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/giotthekk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gwfdtrbsw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gikxcwkbh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gnoaequvl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guschynbk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gyawtfmws.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gphethexn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gxgmenrnx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/grdvljikc.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gikzeaewu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/ghtiiwyxf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gwmvtdqbf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghwyzrjlb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/glnoqnrni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcfbuaugx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gkeezfkid.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gdqgssopg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gkpezsikn.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gwicuyjcn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gxbfpbfwi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnogdfeue.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwvehveti.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gipifhdbp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzhwvlsvk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gkdgoolxe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gnrmhbkrx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvhlunqhg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gsbznqqts.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmudcjjnk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gaqfsdsoc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gdwkwuqph.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gcrajdpzu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gvvvxayxl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gabibgixc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gezggqulv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwqkcepg.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gavtnuvjg.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/grcicrmad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gxndejxxh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/grogdihau.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gxeqpaedl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/ghpkxzwob.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gktgyrhwh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/ghmfyrlob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gzfaxuqrz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gauuljtzm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/glqagyago.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/glialwums.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/grsrfgbqw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gohrazhmd.sHtML


<!-- 参考信息 -->