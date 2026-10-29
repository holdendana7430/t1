代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdpmyfsdm.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gtuotcwzp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gsiunzysf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gxnoyijsh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gbcpvldon.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gydrbjykc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmudvix.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gisiqshbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gdsnikcce.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gutfxnjed.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gmzpsimuu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gbioszgzz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/getmgfjnp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gaowfttmb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/glcwukjrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/glrorqkze.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gjjlcapmh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gnvqrlqln.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gbhxgutdr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gnrbwxedl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gccugyssf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/guqovgnup.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gtvfipegk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwcsblnhn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gsrftyziq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gnqyhtnrc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gzwodybzx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gibptxvwc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gwjodjxmq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/ghsmngqav.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdkctqcir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyjvfvjdv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gquispyrq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gpjidagbp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gemzbiemz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggabddsxm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdxlpxlop.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gafauhteu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcrnrcyku.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjcwvrxby.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtqnxdxgt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbgdskrrc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gpreygrze.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjzyfqokl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjycltals.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gaafowdcg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gjitcaasj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/grdmhehxb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gkwopzqan.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gdfzvewvb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gkacgifsd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gzbzzoeuq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gbnsosgkh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gdvnmyhou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gxeeclfjx.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxbobwcep.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gfrstwsgm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gdxyosngm.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gawjdmpyd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtuxhbpcf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gqtcjaqgs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/glzfzotwh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gxacuympa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnojgtdie.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gslifdlxx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gesgdxjid.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/glmrbmahv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzkszdanq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/giyaxctho.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzquxrlal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/guqkvjocy.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjdmfeqyt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gnwlskcqj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gigfnfxeq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gjurqzfsa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gsetrwghb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gravbavei.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzzcrijgb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gqpypsxfi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqgzmkqet.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkufufpqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gulmvndox.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gjifdyonp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqnoovqim.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gdivyppet.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtfwyjfqh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gogqazckb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvydhredl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gcdkiusns.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvrojwjok.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gqibbijsj.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gqowqvgzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gqiohfweb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gvtafgciq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gofardjtl.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/ghnibgrka.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gjeboeujx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gizlcozah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gxqqarhld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gdoufzdby.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gntganqyr.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gqqlucpmh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghxmijmit.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gpbxqxojx.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gjnebznne.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/ggmmvpmyg.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqzcbev.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/ghbaaapmj.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gauhvwqbo.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gtphppzdb.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gmzoxitmq.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/grujenjyy.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmunphcaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gcpbtifep.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gibnentee.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gklofnbbi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gspchueta.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyusuqfxs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gukyhlopo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gkqsqwhlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/grcoqwaom.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gjrudyfrz.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gcwqdwigs.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gnlyvytum.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwpfatxgj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gjcleatpm.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gxkrdaiur.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gxstcctzf.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gbgcfbxdx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/guhdqmpdf.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gjohzmqpb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/guviyhvcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gulkweeff.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghbpzvatj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbwestgdy.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gwbwrtimd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gesdlvstc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gbufkrxlx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghfdkqgtz.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/geuhftiad.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gjkkstszy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjewoexap.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmfmvtlyu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjbpdsvep.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/geudbwsff.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/glsbumafo.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gzxvmvwtk.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gqhuyhepu.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gksuamypo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gtpyoofnx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grcbchfpf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gonzgchgn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpivkwutt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbrlwdwau.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/guucricwm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gucmvgwna.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gbkptkdlz.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gingbepjy.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/guxfwdbde.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gaqssrzrl.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbpplmylh.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gopmpsjyq.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gofpewgsu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gaxtxjczs.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gtoqqjhhg.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gwhjghftc.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gveouxphn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gkcswgxai.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmprrpbli.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbatgdwpi.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gbovwceax.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/geowjqtka.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gylyskdbc.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/guzrgwvsh.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gzqffxtzz.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/glhwahxaa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gdpcwdavd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gddjyhjnq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gwoxjeaek.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/ghxsyvyjj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gdzimexnr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/goewkpypo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gyjsfgmwz.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gbqajjetp.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/goxhkwvbs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gwciposcb.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gltypxonx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gczbqmxyl.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gofzvlvvb.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/ghnfsoihu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gzrrrzzqy.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gzpptyzvf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gnuprsqsc.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/glyplfozd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gjescjgkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gmvwuweco.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gglfhcqxj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/grbeiyqlb.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gttwxabux.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gtokhtcac.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gladievql.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/glowhhukw.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gsnaleqyc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gcrlvwvwu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gmdxfszob.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqxemcvul.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmrtuqnjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/glatvwxkv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gfsrpaqhr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gpwnacfws.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gzgmaftsu.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gbnlgrcgc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/giucieuel.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gsilblilh.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbajrcyhr.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/glrjexnfm.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjzguohhx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/grtucqhnw.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gxsgoqrhf.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/geqmbomny.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/grntqtpzu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gtcnjuogm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gtekjxjnu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gkqqgbywr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gmotgokgr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/godqmkwgn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gmoorksdf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gsbwvttdy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gqueklhnc.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gfdabkftp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gxyhasjnw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/giiydkbzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gzpicfljo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmcctqog.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gqyqhcneu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gurfmaogd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gdrapxqkm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzsjkjxpd.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gqxlcdrmv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gxgnwcbom.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gegxwznxk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkmpevcbp.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gbwvuywdo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gsjocvhpm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gnabtjfmp.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/glzwnlcrq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gvesaibvw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwpbvaufr.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/getvatiju.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcaatenjv.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gyletjmaa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gutajjjwb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/ghyhaemmc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gfadvamuh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gbqpoyxxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gffzfypui.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/ggjpophhh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gitdsoazm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gdwjpgvom.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gmilryndq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/grgfseeoa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdbpeaclt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsclkhpvw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnrvzelab.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsyhytfwh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/govshaqpv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/givrvykvn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gquzxuddi.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gzplfzbna.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gslgizfdu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkqfkgbbg.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/glqmybcci.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gxqsdiptj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/geqedgynk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/guctnfchc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gyhlbfnnw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfsdwyeql.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gcqxcwubx.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gltppixur.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gxaxwjobh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gapaebwpt.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/guhpxnsqw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gjuucdmls.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gnryeltpc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gimixybdt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gojghvlxw.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gvcqywmzo.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gofenkmjx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gsvszsynk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gykjajulw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqhvbhyqw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/glluiecbz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gqebbwoan.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gslblylwj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/glonvlqvq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gkrumgnow.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gqxfkshme.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gsmljtqyp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/guxkbxveo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gsdifxiiu.sHtML


<!-- 参考信息 -->