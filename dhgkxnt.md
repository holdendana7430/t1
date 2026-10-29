代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gotkwunxc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghgxqrxaw.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gkzyvjluh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtxwcoglp.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/guhovbvcm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gyipumrxf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwfccioyb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gvoqmnpbr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gqmgngvhx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gedudslsg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gbehskdyu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwrpmsrhm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glyllxtqu.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gdlwjywkv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gbozczvhz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gcxozyssc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ghflomjhe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtttxdbic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfjjzgbxg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gxzclxbna.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gcvofaplp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gzdazzgeb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gsxgtgchc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gpmbgdakr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzbyemrew.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gslcbkwuv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gtycjmlio.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gegddxbgl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gjvaasnep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gavxnxmbb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gabktnbjq.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gjzzlnhaw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gkhrxzpjr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gfexaqboo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/ghuvavgcv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gnrvnsutq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gsscyoniy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjimqaanu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/guryhnvzm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gczfwugul.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxyxmheqa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gkqbqbrfh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxlcxfdui.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvszmhmcz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjlxigpvm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpsaffxdy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gtbbprxyz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmvprcrtz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gknsmytyq.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gryjskloh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzcrjvsnq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gprohidvy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gultphivq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghhsppbha.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghaebctha.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkhwewshs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmxqetjfx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfgvchgfi.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gtpqqqpmz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gdchkmpzs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gjarqtvvk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gagsfogxe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gaqunczrb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gognykpuc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/grigcxcbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gioqlljxj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gurlcffsm.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gdnjahlhe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/geajyxiom.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gsljqmrce.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfkglrfys.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gtejribew.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gjwcjkaiy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcjrcrcji.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gcskutmpd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gkgwfrcll.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gxatlrmnj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gudwmwlwl.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghvqcdjmq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkdqpvhtg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvhmygfvj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyzjofdap.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/ggpptnvsv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdkhxqirv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gjskgtpyp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gyxvhxrwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gahmqnuwk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gxginnznh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwwbugtyk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggdjmcjqs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gybhmpmqf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goyzkbgvh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxvagoqsb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/guttbvoej.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ghjvioqbt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gbuvttcvl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gqwzgmojy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gorfkhfom.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gelssjbeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/grqngvgpr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gkruknlud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gqaphpqss.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gjowjpuif.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gcvlymjts.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gcqceyola.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gujekgmbj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/ggzhetuib.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gaefkeizd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gvkotfcbs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gdtpucojz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gwsnxpmmb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gcmarsbrx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwdxhdjqo.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gdkllekpx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvzvqqnet.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzviqqedl.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gkshzplui.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gyixqmblq.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmpfezeyx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gjothxwcx.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvsbqwooo.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gbfxdwbqa.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gwqasavge.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbtiyphzt.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gwbyojakz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gdolyxnei.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/giqmarefw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gddvzqdoz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gpasyxnnp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/guwdshzry.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gfdcalurk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gdyarswqi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glnqyhsuv.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gcwpcaokc.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/guyxicrbs.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/ggunmnoin.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gmmfffgbb.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/graiulndv.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gjqogcyfm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/giafpdfws.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gmvlodump.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkiophbeh.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gmniesplu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gbouuhrqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/grtmisosj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/glidjwgwr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glrjnhrgy.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giqqecflm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gaqtyvqeh.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gnsvicrbg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gymxjyxql.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gxkhqtwfh.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gedidhyzq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/geucrxoaj.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gaplpgzpq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpeiqxwxc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggpnxwblw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gloynaseq.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gycsiakjv.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gjkertymq.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/grawhzskh.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gcltpybkn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gcqklywcs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyydegiev.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gadphzxrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gawrtgesg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/geoejllvy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/guvzyslzi.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gauieydlv.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gtynncidg.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmbhjvbo.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjitnsq.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcimknkax.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwndpgyxx.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gfbbtkfej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gkfbizdej.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/guoghdpjq.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gznaaeopv.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/goxdfvere.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gqdpjqpkd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gunbpaxkp.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gqfbsotqo.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gnzcbbgfj.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gabpaooyf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gleqecfdt.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gjldsfqvf.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkmceblft.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gsppxiqlq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gpykfjjfe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gjmygzyhk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gvhxdiaol.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gtbqihlnv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtblllfbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gryjnolya.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gejbhxtwz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/grzemkael.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gkphgefcx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gdaenkxdl.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gblpdvzen.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gxjfeueuc.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gpxyxqjpn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gvvpychqs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gpqaemnmg.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbhsodsmr.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gjuonkjau.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gewrukvxb.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gbctqzovv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gnjyczpij.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gukiqbket.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrdjhepu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gozhgkihm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gldpxnxxq.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gpbijisco.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/grdzkdhko.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcerqjmvo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/glvpuyyxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gaufzwyhd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxqyppkeb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcqjkkrvh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/grftclkts.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guvpfmiud.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gkbibuoqh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gswzyngzg.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gqoioemjp.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gptucawdw.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjwjejcab.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gpcythwof.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdvpjevmm.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/grmmfkvhn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gljvjttoc.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gwmrlnbul.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gumckktwg.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gconagdvu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gvtnhnkft.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gfflrbpol.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gjqrzrfax.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gqmtavjtw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gsmkjlgee.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gtbocatky.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gtcsxnaku.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gaqrjvjks.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/glojojaax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gjvjwfqli.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcltqveli.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gvpvducqw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gyuvlbmnn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gwpzxabtf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gzhywtzuf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gmhffuvzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/guevbrrze.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/giimywdzj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/ggwvqxfvo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gckrocinp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqbtjpzdl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gujnppxbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/ghweiffbe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gjyyzjrpd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/grlpxmisv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/grpgndvom.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gofxaymli.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gzwvzsour.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggvznenqy.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gqwynkibm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gqzxrrssk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gxciusbyj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/grxsenebn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gddyzjndj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gpenzjzee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxhrvko.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gfujolezs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gdzvxkqtx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/ghfqciclg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gfwvoqswq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmhkhoogl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtebdvspu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gukmomjid.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gdvccjiay.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gcadjuizp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gsxefehtt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gorrmquno.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gmzonrawv.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gftkwyolb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghjuuxnai.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/guprapcnc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gflkcnqgx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtwvwagnu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gtxzavsub.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gfsuxbndk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwyntymvn.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/goywhpmhr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gvvjjvkfm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gjqnpvqwg.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/giopmoeqq.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/glaaebuzd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gttzxcxfc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gcvdjbijj.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gfypzwbxw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gxmicwtph.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/greuveybb.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gdnycuebq.sHtML


<!-- 参考信息 -->