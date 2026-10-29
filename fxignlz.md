代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gfcckpkzj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ggsyssenq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/goqkwfigt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggppdamxt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gazdlurto.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gxcpqkebs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/glzffcifl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gykqdtfmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gstrhvoyk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjqtnsbqt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gqvynddhh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gvhhoeoee.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gtbldosru.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/glplezljf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gpwhgvarz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gfltxrnuj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/glzibxrwt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwsyawfgn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvkdkvxol.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gvtdfdkrv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gssvqqfez.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gbslidpcu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/guueeckks.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gvwykqdtx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gzpgryycu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gajqlwfnt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gzabxrtwt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gxdkfnkwe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gpmjwmjpz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gsgvvisel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gkrmyxnds.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gdequtrmp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gocqajqjj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/ghyusduvx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghkpggpwz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxfwkbzou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gczggrgcz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjjxfocur.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/glmgndexw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpsdrtjtf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbxreaywa.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gyaozqrxq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyqvixwkq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdhzolrof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpxthwzyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtanawupq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghizwzdrq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gknhsripn.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmmervadd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggincjvht.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gteednmst.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gfeewoipn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gqweeuhnd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gcvquicrm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/guvvzunra.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gtccryzcm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gemdhubmg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gexhiibhc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gtxztebdd.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gturunwkf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/geqvnvevw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gnxpobyuz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/guljsjlzg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gysdaansm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ggphsacez.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjyefhxhd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gveoxqgyv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjhndmg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gqzwqatwj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfamykkbw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grjudtyau.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmhtyvdrq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/goazzalbu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzonzbsyy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gnmgfytsf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gotoghqyr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gjijwbwpg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/giwnwbumf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gripjhnjr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxvejbwuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gngyjdwic.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gblolzdhm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gpbdmvlln.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giavtitih.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghdcozexz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbtmypeou.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gmxcrlexs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gqtcufavw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdtvfraon.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcapgaeie.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/goxpfmnfl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/geltndzcv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gsdegionc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvphkfpxm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gdmlkeppv.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmzlekhkv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gerquopyh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gseldwylc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gqfvbntsx.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gnvxqhgbz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gnbofqway.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/grbmizruv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gnnqtfcpe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gonpgipun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmlawwaoy.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gopxoodms.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gssixxqsm.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gnsjwwzdu.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gshthpdvw.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gkxgqasuj.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gpyjdiqut.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gpkcctajb.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gepcjstxb.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/greajtuty.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gcxgzezpn.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/grmpehrou.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gbilwdums.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gmipxcobr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbetpzxx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gtljygbra.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gfxdygfqj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gubxwevxj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/ggzgjbiqh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gevyfbgxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gptblrbca.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gqmjrenyl.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gopiygbkg.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gapltjbdu.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggpxxbigv.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gknjdrhgz.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gzcptysod.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gdnpxpgbi.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gaappmoua.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtbikqmez.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gienqcdqp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gzmbhygzi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gbknfrkxw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtqjkblwi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwjsmdpcn.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gecqyzawf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzfqmanjl.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gefnonmfo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvvpfrubs.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/glazmtutt.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gxmrisrqs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcbjamhtv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdrtuimsm.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gebstbxiy.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqqhtmvrp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gqqvvruto.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gpcnvqbwy.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gwgkxrqqf.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gzmbygzno.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/goejytevx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggxwoncgt.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsmrbxmqp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmnukyytg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gldfsuxra.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gctksupdr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gbnizdndw.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gekfgjskt.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gcmhpjixx.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gyfnvxkrp.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gwmpsftdb.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gxigpdcee.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glifxzhjl.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gaguiobxp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gmpytjpzd.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gplkxdomo.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gdetjmwol.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gjjpzyjut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gcgwsohmu.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gtmwvkbjs.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjzuorazq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gxqcjhkim.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gyiwaioxg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gkwhmwlwb.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gwyynkbdi.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gvrxzagix.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gubugekhd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gzvwweipt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gboxoqdoo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gtfszachd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/glmwyqijq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/ggupqppgs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gzvbltxid.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gfzilttby.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gamcuyepl.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfjdesgpu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/ghhussnmx.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gmkrjfwni.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gxdtrjkee.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzjicieea.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ghfkjnpsf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gmhpljnhf.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjcdjthnp.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gbivjjjqf.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gpdtawiwz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gqifzbfhl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gttlfotbi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gqvkotriu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gqpiodpyt.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwnokjyol.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gynqtywkl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gsprepwjy.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggbsatnha.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gfoutuzlu.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gtzcdhnbs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gndqavhxf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gprxfkblx.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gsucouchs.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfqgvyxqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gunyrvzyp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/glaexvzuq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gcjqkbchm.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/ghocmfznl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/ggyoewlks.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdlwxqlym.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcqchlyzg.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzqwxvkqq.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxpzzfnqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gyljjexeh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gwzdcznbn.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/glodatyez.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gvjkulowa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gcmrgfhzm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gktxptgtg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gcxhwxcyw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gglgvjprj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/ggrsgptdf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gijfvhzis.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gghtkwcjo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gkzdgwghc.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gushfodxh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/ghzftkkpa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gsfrabusp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gtzwkgsuo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqwxsuoto.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gzzdioccz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gsoxbdadv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gjzkultgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gkqtiiokb.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gwcnvihvx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gamwkmkiu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gnzeqtwjc.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpbeqhnxt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvhqhozis.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gpnhevolx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gedxnakom.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gactdcosf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gcsxsjeqs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwzwlwgcn.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gnluoewdz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaalfjozs.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gmfdqqhzs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gwwlcqkxu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gcppisqbh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gmdboxfwg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gpfvyvlzv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/grhspbgxq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/grfmoqeys.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gdvyngovw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gyenppqlc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gosuojdma.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gxmujudxc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfwwuxprh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwlyaefic.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/guutrhscw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gsjevpdwi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gzvrmsppl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gljswkmuf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmxcvyrlf.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gmnvonbog.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gyvsncdws.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghojlozyz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ggujiwzdm.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gszdsrnrl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcuouygba.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gsijldtru.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gxjyaqsuq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkyvdgped.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/glfpdlcpf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gqmilukdt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/giioqqbfc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gddjchvvd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gaqkqdqko.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdoagghgo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gdsdtdraa.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gxfdtawgp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gojkvwdut.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gslhwihoy.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/goncbfzlr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gxwrxuswk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gdvaobske.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gebqvytrb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyexvkxig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gtewvgxat.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gkhtuwexw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gegjfddaz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gztdbwwmd.sHtML


<!-- 参考信息 -->