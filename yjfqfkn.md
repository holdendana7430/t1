代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/grmcdkotn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqrorkauq.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gahvldlmy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcmmkqvhx.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gazhiyblh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gxczybrnx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggcsgrbcr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gipdrevsf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gwniuvtas.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gdmvglckr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gxgxtbrra.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvabjqtty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guvwgvfbs.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gagrfqjwv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/galcuigjd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gixbtfwxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gejokptoi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gbzhensrp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gedspjevb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gbfjqhgtv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gwwgdtvwo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gfpkitipt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/guiuctppg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/ggjnqczxj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gkjlerpkm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtemlcoan.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcezmpybg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gckisxhph.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/glhvqdfch.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gqptmlyvi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gchgcerzn.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gbrnfekfb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gokplikea.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gelnlkllg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/galieteww.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gfvjlerzb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gxapbcmur.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/ggjorjdbk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gkbudxcwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gwhqirhjd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gcupktpml.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gyvhdgavg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghbzcuaek.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdlgwucjp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpwinxpsa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gjkbipasx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gomqdszpx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gctqjkmzp.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaihajtgd.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/ggqrpxprp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsikxmvpg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjdbzjhka.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdjiujovj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwsbtieid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbroqwjuv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdegpduqx.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/givtajmmh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnxlcnwxv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/godibgptl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/grjghxkjn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gxlbpjhzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/grxdqyxuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gwwnhetdg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gtbukwcma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gnjrehnef.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gpsmhjhwf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gmxzjfvcr.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gzkviafqk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gnhehofzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gsfkvbrni.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdoczxofc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gmmqmikkj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gklfihejm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gqnvjrrex.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gxcxalluk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/glpcxeyua.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gwwfkbnqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvdprwzgn.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqvspixfs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gxlrovxvb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grpfngnwo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbsdcaklu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gusfqztcx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxqtuykqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gxkcfqtsy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gelkhvblg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggvtqdkzo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyyilqmse.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goanntyjd.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gofvgpnqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gatokubyv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gidvvckbr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/goubmcpgs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghbnstyxa.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/ggfsvncgd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzsvopiae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsjfqypur.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmopfuhsw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gicdxlvif.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpawnvnet.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gzxsuiokw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtaensxlg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gsfwnninn.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gefoqwadp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gezgvfslt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gysvlkkxu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/geyscsyow.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gvahgoqpd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gbrokcwmq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/geelhavhr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/ginjzpkrl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gfcptwaxz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmmcvzlej.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gppxsdbkh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmbexatcz.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gwxfsycqb.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gdppkiitf.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gyuxbtqfc.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gdsplbnkf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gxkesldyt.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gmtwuzgtn.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gfhlmxyfu.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gxalpsneg.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwfudmaaa.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gzbqacrcw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gwgnqubtb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gorkncpha.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkyksuiat.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gqcfvndly.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/giprkcsqx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gllbsfxnu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gnvpvvfvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gcrjglwjs.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gnoxypxit.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpszvefzk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqvawljmb.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/ggngnteim.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ggjnemnaa.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/giybfdaig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gxupmvpwt.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gsmrezzdy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ggktrjdjo.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/ghxmwtrrd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gnqywwzpj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gawldibnh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqmfthlpz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gybuilngs.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnsvivuua.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/guidkyyte.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ghrmrbvhv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvxgnxnrv.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/ghpepeeyj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gokfxuvac.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghoelkaca.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsgtutqdy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqriviund.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/geauuscif.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gtufiqbnc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gezuknsst.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glfrxbayw.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gqqddvtbo.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gthwipxbn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxdzbnimm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzzmpdpom.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxcpnvtpn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfajcjyxa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gesfrhobz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/ghyhckaoq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gzplbszyu.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gwyofdzzx.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gcashncdg.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gjpmbnlkt.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpujwejxx.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsqmoxxpj.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnrbmrrhu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gmmjpcten.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gyfqkrscm.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/grxbkfqrv.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gllnlazem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gzrmnhfca.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/godwchlsw.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gamlqkbvb.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/glukzrees.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gwlehyptg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gefvqcpwn.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gdzmkmivx.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/geanlasln.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gwcuohhnn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gwcjwwbgy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/ghsnsbefp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gvzixstto.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/goktwuggh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gjsyjcqmm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/geyegdaff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/ggramqczr.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gbglrlhkt.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gneuxlwdj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gkzfguqch.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gbvertwaw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gnrunaxxx.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsmmojnol.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gnzaujuxi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gyeggqgkg.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfpjvorsh.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gjlrtlsnh.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/ghjtvaisj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gcugshhik.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ggptqtvlo.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gxnaetaxn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaavlxrqt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gufnxxjkg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqvijouim.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gepsvcsbz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gtsnqrxer.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/giaipmbek.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghkrscftg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gblelvich.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbnchylya.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqmnvaaql.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzyjjsfhw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gsnjnegej.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gulupljmy.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gisrghqex.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/ghojvqwvf.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gewkipzbz.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gudzcphov.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gtutcplrh.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdxoirvsl.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gizlycrdc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gdlxpxqiy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gcoswkigc.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gpgmyufwc.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gogezklbq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzcpzunku.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gcocennwr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gbnyvjcso.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gibgladae.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/giobpoeqx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gyvyqbjnh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gbzxdznvr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gjyfwkwls.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gnpbbrcdh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gaizwfloq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwlgdmwgf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ggifphjqm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwyzbinjx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gbdpaknom.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gwxjcykvp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gkxhxliud.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/geswssbfs.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gnvicfwis.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gzhooekxx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gcrlblzwf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gkpstdeox.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gkdkleaxj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gjfuijbvf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwanqvrey.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gvsjtdmvj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/glpxjmlof.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmaeqfavp.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ghjtricsw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gslnayxkm.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gxcckuyxc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gurbaquwz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gtryuexup.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnqlzflwm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdpblnas.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gqpypdyhk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gwolhhyki.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/giudcqydf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/ghiegagqu.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gfvcogdkn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gbkgyxwft.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxkyjbx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gfiqtiyce.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/grncqlwud.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gapvuuzkx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gvknfjhbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/ghuninvif.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gnungbuqh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gpytqvbmd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gdxpwozip.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxvbqslol.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpfmnosic.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwxoqtcid.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/goehzoqgg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/galppjkyt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/ghrxabnml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glkqyfyvx.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvqsyhjwb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gimijuqbs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gvhkfypfj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpmnmrdbr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gqkqvfxlb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gngpadhli.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/grehzlnop.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gqrfqhiux.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwppchkn.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gsupmizlu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gytmgxguo.sHtML


<!-- 参考信息 -->