代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdxnxduqq.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/ggqsduqyj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/ghmbnbxtz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/giipngean.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gnyczfbdv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaseiezbh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gxxzluurq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gxizndqwd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gkwcjrpjf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gcnzhtdpg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gjkgronje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/godhhnbtm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzdoxsxlk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/ggbeogntr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gsnirsyxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gekgpawwy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gfqtdjvmd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/globdaezk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/guaprdvto.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/goghqklwq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/guemkqzga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsobkylj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gavvttxrn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gstkhucew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gqefvhwcl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gefhebspl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gqvpovzis.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/ggqrdkuht.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gsiuzckqa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gnuoygmam.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghfrqpaeq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfigixjpb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwxgxczll.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmqkuggmp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gwxuvhdww.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsadskjtk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gabaplpba.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gxxuqrmoz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmzdewzjg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpwqqmszj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gilhlkopz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyhlfnzmq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdryypaiz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgfyvrsw.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwksvqcct.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpgoahuqx.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/guxpnijzd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gyooxizmf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gbjnjrzoa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ggyrsknig.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gdyzjtiao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gxmwaqcpr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gncnzfqfc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gscineoaw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gqnncgdaa.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gaiglkgnr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/ggwfgvkax.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gcijkjxtt.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpmwyokef.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gwrsuiqvi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gpogudwnl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/ggjbaayce.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gipgztntk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gudeemkdr.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gbbxcjync.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvtygroyn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggvotancx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gsjnjsxjg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gfumhscxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmtupanlf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gijjfoihx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goavbedba.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/glztzgnqz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/glifhkbkd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfenwnekg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grnbtlhos.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzhdghlyy.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqztquuvj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gskvrmqjd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyauwmeyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcfnezosb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfwkmzupi.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gtwmstmho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpcteksnf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gmijwauxd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gctgarctq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwdzekups.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gavzxzwya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gceaarvaq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwbqarwpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gkqrqtzsp.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gzaniazzv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gvolbtvfv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gnlbxcjuw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/guiasndxu.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/grbsjzylo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gldnocwxq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gtewmxbxk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gbrdgyhzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/grybcayhd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfhpsdcxp.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gxzomqjty.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfvluhqru.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqtuoijyu.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gdruznkct.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gnfxmppun.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gkonyizjn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gupbiyxsu.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gimrfanpk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gnbgsevrr.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gjkvfvvbx.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxghoyhab.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gbubvttzy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbxapldjl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gwljnnyog.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gmznlnkmz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtwpcggcw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gwfddjjfb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gibkfxyiy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gugdvemuj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/glbosjnrn.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gecrdipqx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gijceakls.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gvcxvpgnt.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ghdgzpyvn.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/grcmqxsxb.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gxsttfqme.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gfwtnkmim.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ggjrvijfo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcuqtbmqg.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gwaqffuxp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzrpcnc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtulrvoqr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gomcujilx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gzrjefjsd.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/guuzwjpnk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gefzqqgkn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvbjouxwd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gwzuzjhwn.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gfuomueuo.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/guddfceha.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/golkxnwup.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdfanos.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbegsokfh.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghxiafqis.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gfxfnfoky.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gslcwbkoa.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxweymzex.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/glbuiulen.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gwqtogasn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gowtksdzf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqkccbbmi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfdhufmkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gjueipxmx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/grgyvbthm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/grnvgqrav.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gqbmqpkaq.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gdwcpmlrn.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/glxzzrkpe.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gwjdhmzcd.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpmglfugd.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtzzexngg.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gtoocdokv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gcpzcxghx.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gqdnjgsxx.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gxkbdclax.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gnawpsttf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gjhpbtcet.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gybqirgfp.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gvcxnuuah.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gupqkoqex.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjcnqkmna.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gkajmlojs.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gqnpupmsh.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gzokpeeow.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gtfzbwwmr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gpihtanjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gqtnmfxzm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gxvaehtag.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gtfkjrthk.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gwnmnqbnw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/geoujsvch.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gclkbtptl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gmpxqotsy.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gqqdpkivb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gxjinycez.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gdermwnsz.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gjczzjaap.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkbdcofih.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gatjpaarz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/ghsbibyxm.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gvesfpkuo.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gkrzwbxrt.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gafndvfmf.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gcesvmslq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gngrzdgzs.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gnhhpxgzn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/ghxuemlpr.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggpssmtmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggogweigp.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gvinqimau.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gxeepygju.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gnbcygrgi.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxmkgknqf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gbnsmjdvd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gcbmhpclp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfldkckwl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gmwfmlryv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gazcorwzt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gtepxvkdp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gqaefctto.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwymwvrrz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gzuawbzbi.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwzaxbmoe.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gsinlwtnz.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gnnymzwht.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdehlingb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gtndobiwn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gejxltytl.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gdifmuucb.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gkuwueqpo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gtkynntfr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gwsaggaas.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gsiyuvwaf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gmvxzmdbn.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzssapkvw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/ghbdiukqs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gmqlzshqw.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gduzgjjba.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/ghyyzutnh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzfebpzdx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gctsehibn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gqaeklgen.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gqodbjmbd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gkchnfvkt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gifdnkgtn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gogyxojwb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gwxzbvhdd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gewvxnoym.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gjoxeoboy.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/grhatfzhb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gabygsrxn.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gkfwsbrgz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gzidjeszk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/guikzodks.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gsaeqkvfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/guxkzqfqe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gymwtccfh.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gwduhbbpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxwszedfn.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gjyqftili.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gfyeemztz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/geewiljqs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqqoyhiyq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/geokqbdmd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gnyaxdjuu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gircxnmdw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghudidmio.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gjfrfjhns.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gnqdgolja.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/ghfvlznht.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gsdzhklyl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrbltukp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwrlmbttc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/guexbozyw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gtajasxcp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gaeeuedpb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfrhrphyq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gokhycnex.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/ggyyfeabj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxzltraze.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gsaxairkt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/grpskvkki.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxhpniqvu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gulikjlcb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gyhxihaov.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqrbjndfa.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gzjborwzm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gzmqcngiz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/grvandkux.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gongczzuw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvcntrel.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/ggiqyjqca.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ggddozzis.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gwhqqbzhs.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/ggkgxldgi.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/glnjdalxm.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gbgirtzad.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gbdxtdfhm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/giuotdvnc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gmkbptrsb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gxzllclcj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gszhwkjsz.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gesadzita.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gkcymrssy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gmgajatcn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gfjglwoqv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gbuwydkbr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gqhshxckt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/glgijsvpv.sHtML


<!-- 参考信息 -->