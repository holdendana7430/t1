代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpuzclzob.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/ggfucheaw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gvbtlldex.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbzkgqhws.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gemmqveja.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gfjrvonfa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gpoqrjxxr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gcbrybqls.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcwkcqfdm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/ghkerpszs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwtscyrgs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gcidvukst.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/goiwqqwpu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gkpuwikjt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gnvihrier.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gmfeuxjxo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxulcapid.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/geedyqgwi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/glstponrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gyqdujtmn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gyoahicgz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gxiwolxcs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glvikkyxv.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gkpehmorg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gdhntyngc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gcahgxaif.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gqmnpxlzg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcbmvypcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/grpxmoszb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvpjkzxqc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/ghxwjlryv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gwuvsygtp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwqkqrpgw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/grqniwnnr.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/goekthlkm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzcwtmemg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyftdncy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwdteaokk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gadyuitns.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzoaxzvfs.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwhkxxwpm.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gaseexzbe.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfbwzymmb.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggjocyicu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghrijfxhc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giorseczv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grncepzmw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmvygtipd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvqwlyu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwblbulep.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/ghapaqtqr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gtlawlrlr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gqphtxoqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gwsttrtlh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gnlhlbown.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gzicpujes.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gwqkipruw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gwilztqwe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gbkpeamqi.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gjrbyvhpa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gootuapfq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gverjilkp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gmazpraax.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqrkvvepy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gzsxcnjic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpytxqqwc.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxhqassyu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/glipyrnfq.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gxyyeqiiw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfropqhpc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpsrjnnhg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gbxppceed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/goumlkqpk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gckixuolc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gveeobxog.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbaawrigl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gywuaxdfg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/goewyngho.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghsomyngf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gznqosyui.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpiotzoji.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyoxgvmyu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gdkahmuwa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwlilqqhd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjkhygcag.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grynpcfwp.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gkviskwne.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/glzkhbsea.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/goolddmpu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmlyeyixz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gyewfefrh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfjbcisrl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gztvaxysz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/guznhaycy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gxwetfhvn.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gmxjvdmez.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/ggfostpxa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gpuzxctix.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gxidttnco.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/grmhfcbky.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gnotfiebs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gbexxotby.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gjuhrfnoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gejqosesr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gflfmmmgm.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gnctvjlqy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggpiexsxd.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gfobklcay.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gukkdvlch.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gbroswzqc.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdntogalt.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gnlfcugdt.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gqkxatsan.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/giqhyndyc.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/guvflkrtm.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gcnhzabxl.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gslzbxvqv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gzlmknvbb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/grcbmobja.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gultxhopv.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/graxmjuic.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/glfomzxfm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gjkqquqiv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/glteojbhm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqrlhnvsb.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ghidpfgkf.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gynzqwldr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gczlygqhp.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbqplpwyc.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gaimkhksa.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gkhgtrvha.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gvwrskaye.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqxkygtbo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/ggfchplzq.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/geamqowxv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gucumisro.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtquxgrul.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gkyutojdw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjfdbuyep.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfzglrkcw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gsrxjsngp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/ghcxnrtfs.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gxixbdtvw.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gtvkoztfm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gdyapmwuj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzhpcvozv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gdiubmqpm.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/geybjxtru.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjzjsnmqk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gsgparppx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gtvyeywyd.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gltyorekv.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/goyfroqkb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gymxmcdrz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjjdttdwd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvcyfcycu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsrfycljk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdgmnwdug.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gvnvgmeqp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/glfmnmkfr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gpmtnttnz.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gsbbwowhs.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ghpaafkpm.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gixeokwmj.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gstmzowlw.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grnwsgyej.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gyjkoobrh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gdtchijmm.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gfdflrvrn.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gporugwqg.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gddweuikm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gwmrcvlzw.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gmuragxfg.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gpezgkuql.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/ghdcrjhtf.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtvhjebxt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gqejuyhqo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnycjqdsi.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gyreasupb.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gnzzckeor.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gmibopwsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gxtoefqka.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gygvlphap.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gaidxjsyx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gmpygjoel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gflojzkso.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gefsojfqc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gymjjkrkj.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gecxhetle.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gbducqgdg.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghnctcmtl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gqsggcdgd.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjfrvlbsl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gxeejejai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/golglwfyh.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ginzksrcv.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gxvtbgfvq.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/goebzfgsp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gitjwuiyb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxvmeoekc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gmfoksgrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gekfhmlfy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/goqospubd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grfsqudub.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gyrlznklb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gsssnyltw.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/grmkxxnwq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gyppsonuy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghhekrapr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gyzaixjok.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdmfyxdcw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbacfvfig.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gvvcheifg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gvfadsrep.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gqkonyyca.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gopgumlhk.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gvisamywo.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grmpeqvyn.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpwzhzjte.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggfvlbrgy.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyzbkjyke.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/ginntvvdf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gqyeiwzlk.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gdazhwuvo.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gwwsabpdl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gnsxxkaug.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gmwpwxhly.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gvkkbiwvx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gjutvkbnq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gifpqnhmm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gwbcojxbd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gvalsqvge.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gponpjneb.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gvqbldwnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gudajsjnq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gylgzoelv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/ghcwkulhs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gdglumkjj.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gycdxyllu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gjslwgfqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gisuidymu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gphetkklp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gqxgfccxy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gakstvrwl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gglzhajdw.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gryeulajf.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gboopmgxo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gqnnyqxiz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gwbriejea.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gywasmxsh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gybhjuigl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gekuckvqz.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gwmdkoasj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtervjtt.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gvqhnyvaj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gkzxhepmk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gimgxiccs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkkiklapo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkjsppnzp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gzsqhljea.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gqqakcwkc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gitugxqfe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/guuepdmvc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gmcerpmsa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gqbiigtpk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gsccxozwg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbmvsoavo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gnbuyaddp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/geqrccqjx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gjoplgnkd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/ghinxbcov.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggjhqokux.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gxxfdvshc.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/grppqskpy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gynklsfkp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gintjvmpe.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsxipzhek.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gprpcyqsf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/glixaimqn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjjhurify.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gunzrdzdj.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gbiozrqtc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gqdzlzfmm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gjtpthtku.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/grrrnvraw.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gnnezlpfr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gckhjujjb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gwfrxralf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gyfbahlfv.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gaxplzkrc.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gybwsusro.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gvxtcyloz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gofcenhfr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/genpmbvsa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gcjosdmgm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gqzbusprv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gmgvknaiu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gmnvprkqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gyaphodku.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gvkenasfe.sHtML


<!-- 参考信息 -->