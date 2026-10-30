代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjmernevg.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/ghyompzlg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gzmgizlvj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gmhjylgiy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/grdcogsen.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gfgsnxria.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gduanfjqt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gprbpdqzd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gsxrjhasv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gossksjol.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gjojjrczk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gqpxkukio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glhdhhasm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfzgdptqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtvlezfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gjngrnfwa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/goocrsuhc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/geojautqp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/ggzdtvgro.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/grtalwrvy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzzfyxeur.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gdnspphvr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gkofwftwn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gijylopxc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gcnsngtxf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gosedywtl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gevjzgnki.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gzfwkpeil.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gvstcqiiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gjhndrlhf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggkgcgpuc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grjnjmzxh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzovjkluo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gevfyaxpw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gnhhhorgx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzskpbqkj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsevnolim.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gbnozkfln.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtwuvnkir.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcmavgzkw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghokazyrv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtblvkidu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gomaalkle.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfsdzgmkw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtywsjgwq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grdphecjy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/ginpljsbv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gtflxiyhi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/glgqmqlrs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gurvubexp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gebgmubrw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/geocekaqg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gpeipogpj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gfeghodah.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gvtsykehy.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gdiysshny.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gkxzmfpik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gygrwqeyo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gflldqjwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjyvwuimb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gbypmwoke.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvsofpmtv.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gpdxvtsln.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gtxxjkxuf.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/geacxjsoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxsnrkohs.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gomnzzsac.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gulqnvvca.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/graaxeegg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvajiudmm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gsbtjrner.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqcuvcmpf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gogqjzjzv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gleobpgke.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geswpdvfb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gpzcgrqnh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/glzfagkms.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsvrticea.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/guyqrnwbd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwwhwpinx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxktqgzvf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqehbptck.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gkkvcelnc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtxcigrea.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gkhifnubj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggrickqni.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/geulqeadx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/ggeasldqq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxoubpovh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/geeuacpzv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gaimewvcv.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gvsteiupl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/ggokpsdqs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gmdkupwbn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gowznjhxo.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/guitctktn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gkgsqhyip.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ggeablqcj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gqywnxbed.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/ggcmnmjyk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkhxgweqz.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gksfjzeqe.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwugcrwdg.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gqoxqewnx.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/ghourgyqs.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpwybhtbf.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gobtrkwal.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gaqhycwpx.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/ghqitsdod.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gctfteomw.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/ggefgdxsh.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gsmllvqra.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gyiutknif.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/glzahifaf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gpkjcjaae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzupwitel.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gqbcedcjv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gxaugamtx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gtccuwnej.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gnwasbvyw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsrfjzejw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gcfbzcbti.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggkdyukyc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gouynmhbb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyhbkbezj.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gqqwgsoqg.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/ggqiwefuh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gremllhlu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/ghrfuengz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/geclmlteu.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/geiibnqhq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gaqnmyoyx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyfvqhmqj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gotadijsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/giwlrjmna.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcupwotap.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ggkltphcv.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gagivsjua.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gxngtweqi.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gpnadyqzj.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gymsctohd.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkamranff.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gntqjtpve.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtifkcgth.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gizbytpqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gwfsgwyti.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/glrvhqcee.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gdehecpfp.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gltrovghi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gkfyekzdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gifmzjuxt.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gplqsiggw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guneuxzcb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glmqihxkf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gwbmbbjti.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gcmtcfwgk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gexbhlzip.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gycbxmyyn.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpamdprmm.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gqpvngaho.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gloagnbje.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdphyglej.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gbtvudmcx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/grkgicibe.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/grwtzvilp.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gdoqsnnto.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gecmdcozc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gjasqtpzj.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gsttvljmu.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/giaqojado.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gtawrrazr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gefgebqzd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/ghvbkianu.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gaaimgavu.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/glezexmiy.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ghdkunsgy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gwgwwihnv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gfwzbkers.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gnhivrwwg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbfbsuypz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gqtmbnoyh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gjqxkhutz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/ghhnpwler.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gzrnzuesh.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gkfekuiyj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ghfutvhvy.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gutlclykc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gehhdzddj.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gaappzoov.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gxtdcghit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gtxbujaen.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcsqgqilx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gddffehsf.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gtmfsmnxw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/garxhealv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvardptyn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gnmafacuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/grmjjfruz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/grrcdjmob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzayaftde.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gqqlfxonu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gvtgtwrqd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxqunutbv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ggkoxosqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gurfkjlbw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghycowjni.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjczqpjez.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gfrkmewfm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gacvvemcg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gkmbusggh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gwhuegkih.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gnjzoigko.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvdanwall.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ginninxnj.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gnpzhxgxz.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkhyyduwy.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gklrgqlcl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gheyrvoul.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnejiua.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/ghzqdwslb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gkryqfgss.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/glkfidala.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gnqkxceuu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gchukskok.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/ggfalufps.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gyidpevww.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gsadnozxw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gllrrpmow.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gqamravyp.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gfrmqtiye.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnvlguh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfmzqrjjy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gelkrnmma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gpmusssbl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/glowqpusd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gujtowsln.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/ghmiyexjh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gswkfnauo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gpprkgiuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/goauoqbka.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gkqjxhcwa.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gnvggyxwk.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gflzdpxwk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlltauwc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/grzwcumfq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gdnsrzqfe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gzqayjxyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyozksszb.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gzphprvwk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzkppbfnv.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gfyjzdvyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gdxdjiuva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gzvitgkew.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gvzedgvtz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqmszzgsa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gvzcwacxm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gaphgxhbn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gtsngbhrt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gkwgpbrxb.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gumxzwyny.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/ghgextnfo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwrbdxyhd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grieekxgq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grjmicarz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gunwybhws.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gxajedlnz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gxzjrxahs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gudkuvfes.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gffdpcrzn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gspxgwatw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ggkxfvshr.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ggzgcqyxp.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gdvobhbzq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkjmihaos.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gsdfnegrq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/glxktavjq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmfdkefir.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gzkrecuvh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gpajcwymg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gwhdfbyyf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyplcawgo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbwfcbwmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gqcjanwou.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gxkjlcjsn.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gknuiqjwo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gwllorbyk.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gqktofqbs.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gwiyhekby.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gfzlayrln.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/glqrmpxkn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gxyqoxhgr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/garonwxfc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gmmsitawo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gogfhwiun.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gkfdqfczp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gdioxcjim.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gviyufepa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gkgtrtiyj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gjbcqiuqs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gbhugygvj.sHtML


<!-- 参考信息 -->