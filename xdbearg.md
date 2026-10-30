代发 wailian999

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gewjhqouj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gwoabdkww.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbfiiaqyv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/giwbskpkg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gmdgtoyfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gopkpfufd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gptpmkmjv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzhdaznsl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gngsogayy.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gminlgvxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gmbvigqpu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/ghxyxntne.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gpvvdzolw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjbaupqi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmvtemxsf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gmfkktqmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gkpwbjgjs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gvolaxvrv.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gmagthjvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gyjwvtxza.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gmgklapeu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gazmkscem.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/getephraw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gdhfpypwm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gftrkgxpm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gnlctpcpc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gknjkhsjv.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gutklsary.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gumvtglrj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gbgppnply.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/glcpjeazd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gosagepsn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gtqizhfwl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gfqwrjkmp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gwagzajcm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/guwtygngy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/glkgyfufc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gbxhmgqgi.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gldacrcxi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gizsummmk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfzqkaojt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzxgomijk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gexkmlpyx.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggdscxkbj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyatfqjza.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/guliskwtu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpedwihze.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkyepxrzh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gteazqojy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gszippxhs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjgomebmn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzlfviptk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxdtalfik.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghpenaprn.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gqhwsxabq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/grexwkxqc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gwfvnfill.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gqxqmbfji.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbcamvisj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ggjxgwqbi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gzmcictei.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gybkwumgb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gcoammldt.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/grariawlg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gtrefoifv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gfotngird.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gchfjkdqw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gnovjffdi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/guicfzwpl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gqocycqnm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvgogdhv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gamdzrkhd.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gxhqmivod.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwxfrbjbb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjvtrywhj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gxrcfmhou.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gjzjzsooq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmiztjlii.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gcjyhulgj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtereteps.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gafjmpnkt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gulzrvjmh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbuhelqrh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyaiacvqi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghoqdrnxj.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxkfmeafu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gwmntfvxm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gojalswfa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfqyqwksd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpxxpctte.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gkdlopyaf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gcrmwvurn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gzjckesyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ghqadycxk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghzfvkrjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gxaktmxtk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gvdprzyjn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmlnawmhz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gzhefyqmk.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gbmogmetb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gdwktbvwm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gayimkpfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/ggvzhjxow.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/grqcxcnpp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gwciaysea.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gsssrcfyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gsaqjqlcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gfeatzjjx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gldcwnydm.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/glqiocvaf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gerfssfsc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gxnpugdiq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/guvefbniv.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gssmepvzi.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gujuxoxdo.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gcxohiavt.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/ggkrbtmyj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gzkcuagzc.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/glpxzbhri.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/giowcpeoj.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gzfgyvdgc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gexiztzti.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gyynctezf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwzdeqwpd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gkaglspzj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gntvvstso.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gvplhyerj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gczfhtrqw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrnqahez.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gsgixozhm.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdmelgrya.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gsgmsmemq.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gyzittiew.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gnlrdphrp.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/glctowsuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gqrsmxmvj.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gvskwysci.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gkafuwzbt.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/glugxvucs.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gkrckmfqm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gkdqmamql.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbjehtdeh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwvdsudje.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjwhtvlgk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glcpszphn.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gyldayylw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gwezphkfl.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gotdzbdjc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gmqpumgvc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpmnaesws.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdufsgvna.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/geyvyzbai.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxtbhcege.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gwjygbrij.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gmjzfhwnm.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gsrvpitpz.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/giimsdygp.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gqdlsixmj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gqwyfxdye.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghtlugkpw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjcyfwiyl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gyeayvual.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gxjpydnfz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnqjwoevl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gcxkqjzpi.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gxhwectir.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gwzxkxcua.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gvcmqqhwe.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gscrmflcw.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grgmfnslu.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gcwkgvzou.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gwgftddup.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gfzqqbiwg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gpvuodywg.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gyjdmpgjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/ggxntscgi.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/guezoylwg.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gtbqwrlru.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gamzvdplz.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gsektkgmk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gpewxwvja.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gbcskvjrd.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gaxbjweeu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gchedwpgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gtmdxucxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/ginwvssbu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/glthylesm.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gbvjnopgx.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gzsvdqwvg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gelvsnsgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gzpbwtspy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwjzthmye.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gopvwfpei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/ghnbqvfmo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gxvkyfzwg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gxhahldnc.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/goxdjilvj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gabgecdll.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gtbmmbxbv.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkacviwiq.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gsxleujxt.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gbwlunkgd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gwfcqdihg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gcvrqaycr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmcncmfqu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gtadzxwcm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjjzxykwx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdkojngoe.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gfbopmyyd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gtdwqpyjo.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/guakzzrqz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjsreizlv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gnoyggwec.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdnhhfexn.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghuprzxdz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpagbbuzv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/glkryfpul.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ggtvcqnhz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvqiqvkbt.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfoveym.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gxsrhgwaa.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtxqxtfmb.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gatkkmrta.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guiiorewi.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbascwupa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gnvajcbev.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gcgttvpkt.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gidakgszu.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gxhyekhdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gwvfiyedl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/giikfmuwd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gycigcnkw.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gyxsqkkdp.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gbgkvcvao.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gdhksnbwb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gtwksbtta.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gmkkidnnp.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gzxnswmik.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gfhgymcjv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gfedhftrq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gauvgyeno.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gaoqqadbg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gfgoxidpk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gsauumhpf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gictxirgu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gglaqmcak.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/ghrigvfyz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gzsnyisqy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gmuuuxenz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/ghkmerdku.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gqrxyaqtj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gvgimctyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gleotckia.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gcegnxkwh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/glvmoqjxq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpfodkszy.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gcpbuenmk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtedlmtwv.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gbhdhwfmn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gvekivldo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gscwtubov.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghukqbfco.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmaptdodm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gwjitslgy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/guihqvwkh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gjczirtbr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gpvpfrwom.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/geifbkdgo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gshueiwtu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghfjadydq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gupfonpop.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpqqezltv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbhikwxzo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gmdxqxrja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gcxyipvns.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggufutcgz.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gkacefuqi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/ggieolmyt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gszzzivjb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grbonjmro.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/giauacvxn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxfjyitcq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gegssefxr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gbfoqkcrx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gthuibxvo.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/googywzqu.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/ghccoafuz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/guahuekfq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gbcpymvvl.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwirwfghm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gwfmrefli.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gezkxfett.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gkizfkthg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gywifxyge.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/grsvyzjhu.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gutuwrknn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gfeojeglk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gczlmpmff.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxwrkqknv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gpjaaxaya.sHtML


<!-- 参考信息 -->