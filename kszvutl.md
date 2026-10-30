代发 wailian999

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gitgkpxwy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/grddhqxbh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvlctvxzm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gowlwogsq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gqjnvnwex.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/giaqsswdj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gqwjxvtkf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grggrkhpc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grfpbelbz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gsmiusamg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gsajrmeza.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gcrkaalhi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gzaugrhts.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/garnqxwqj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmitweiro.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gbdnmjzpx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gnkspjlbu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/ghnyfxhnf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gsuicbcfj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gciyzjgcq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gzekaaywq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvndycdnp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gywlxeuoj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gvceusgot.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gvgubomvf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gxkkfmzxr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqztdkbvt.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gmzeszfie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrufbood.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gbuhrxuor.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/ghhwqojnh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gckoswoqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/ghzjfdkwy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdklmaeuf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gigrcflji.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gfgnhfmdt.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gcqtoheiv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gmfanheqz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaarresil.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gntqyqjsu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsfiijfkv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbliqnubs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gdrboakzy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gukmzjott.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfruelqbi.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/ghozmfade.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glpcokedg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnjevodfg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gexdwlpwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gptuibjep.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gshpgzksa.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gewaeflxr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghvdmlhsq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtjtdmwal.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/guydggbqq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gfvkgbldr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gsvmetbud.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gdykjuvdv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gqfmeoqoo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gwfwxagdg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gxeaycglr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gpvobsacp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/geveqaaeo.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gwccvfdfd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gpnmgtbpt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/ginzflrih.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gobfyutnv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gvolexbjf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gdilgralu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbhuuxzut.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gzuwubjxq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gxplggslj.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gqzfblwjv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjngapeyn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkggjyqgo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gshzklenc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gcjmlcsht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtdsshipy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gmjgzgzws.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/grzxlocxl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gufbpbquv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gbfoeqtef.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzsoarqoz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gynaldbab.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grtflszwc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gakswrgpk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gskufsygg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzrijngyr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gfcagyvks.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ganufjbas.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gdbtfpiaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gffnxsqrx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gzmmswdwf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gukhcqulj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/grvyicetj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzgqhwwti.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gbtecdylq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwxqthbsa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/ggfqjfexn.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gmzwvovhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gpgkqirlk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gevdzxlbc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gcdutsrqy.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gieluyyqq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gljzlzdhv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gkultnlnl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/grzdvptfl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gigwgyrnl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdeflgxwo.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gewdfyesi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvguwdflt.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gryosjpsi.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/guqefqgmf.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/grwkkezym.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggthzieyd.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gqgbymagv.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnghucngl.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gofebsiyb.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/glgutztek.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gfbqfqxxe.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/glvehvrai.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gnewffjnw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gunzgyrya.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gsogosoil.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gfopeqepi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbqjylfwu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/grepybhql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gjjdxyaif.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gpvrwlbar.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gdvkcxqie.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/grnhjrqmh.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gykindlcy.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdtdodl.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gdtzdhqbd.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/ghkmtakef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gassbhcsz.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gahsdeiiy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gdqhxodss.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/glcelwbjb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gjyxjmeug.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gjlrgvmqq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbhmybzya.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gbpkcahgn.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqvakxadm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvdciihtw.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwgwxwvll.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gsruvmbwd.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/glcfllxsq.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gzjgwvrjz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxpphhyyk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gznvloxwh.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvalsbvqs.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxbkwclrq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/glwumtjnb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/golyhzynf.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/giujndxti.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gorlixbaq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gnfgrmxrq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnslpmzuu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grvcbqryr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghvhpibca.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gcjywsxgd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gjdqaxrnf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gyrlacsgl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gykvyibbc.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gmxappohv.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gdgjlqsyg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqbiqlraa.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gesazcitk.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gsxhovjvr.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gniomibmg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gbehhcqzm.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gslikhasr.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gxktwaojx.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gibjkltwv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gxrpvnwus.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/ggdlhcauk.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdxvfhwkc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gpfjhamtn.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gkrfucppa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gcysgrcza.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gunkegulc.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gxpnbuduf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gwbyckjmb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gbrgckibb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gfdpjbuqn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/garnexmzn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gtbxxziir.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gctniuref.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gihiwppbl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/godcldycc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkocbclcm.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ghktmgfkx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gvryydhnu.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gurgxfgfd.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gcbfqtwig.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gwykeoqen.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/ggiboqkzl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gjclnhxvg.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gtvczuquf.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ghedhfbiy.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gvhkkxzni.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gbroajszt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwhukavj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gbajxzzgi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/ghycliaqp.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gefffdfca.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gljdqbzms.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gcluphmaj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gfejvaces.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gnwwncnzq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gqaoaqipx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gicnaoxzo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggbguxvrh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtuplshgb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gawttznnc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gsrssotkw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gvcluolpa.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/geslcfvjk.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/golumnwws.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gedxgentc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkujtfyqz.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxdkrtpog.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvpaouxzy.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gppxatlgs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/grmfrlaqa.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ggqrsjjjk.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/ghuacpjts.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/giszksetc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gzmkkhyei.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gnlmlisbo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/guoyejkwm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gqfpqszox.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcaumfmfh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gsklazwwb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gsfvwzxhy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gswbfsflx.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gosxbfkmz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gusvfmzkf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gfdfxmtks.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gjorhkezf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gaqgqrolb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gsapfvesd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gwwtnquzm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gmrlhaicd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjwjenlhd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ggwonjjwl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gdshdksfk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/glxsqzazk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gglrvqitg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gprnxstmb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ghdguzeqg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gdngojdos.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gwnlyzgen.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gkqrjsrty.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfmojtevl.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/giwdephtc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glhixdfjh.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/ggoywdexu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gtlvalwhc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gukfyenzs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gyliozmnq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gfftxyisg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gsruqocku.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/glypzvhgp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gohchdeys.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/grhpjxzug.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvkkbdb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gotvwmqcr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdxtmqmdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzmsyngrh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpucjjycn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grsfaawdc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/ggvdnqwqi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gahwhvrze.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfcqdlild.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gpidqaxad.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gboxyrxoq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtugztxsb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtojonfvs.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gpelidgkn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gwbbanuux.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gnoznsazw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gxhxylvsw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/goldgzpge.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/grhjeeesr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gxflbxqnz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqwrhqwsw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gmelbzdxs.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gsuginsrf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/grzfidnvo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/ghstgnxon.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gtghgpusw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ghxrheylk.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gpfphkycv.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gszxgjgda.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gpmmznayc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gufqqcper.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnfogsonq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxhncvikc.sHtML


<!-- 参考信息 -->