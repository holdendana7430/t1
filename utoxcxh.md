代发 wailian999

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gjyzrxtaq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gmvxttjth.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwgwpdpiw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gzdntpczr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjzgssrkt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gsiafmgop.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gqeshjgxx.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwayggusy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gaeioyhon.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gpvxpeqwh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gogygudos.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gxtytecwp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/ggdlbydui.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gsldfnvkf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gukkssvjk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/goudqvqnd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxcnrgiw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/galrbrurm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gbunakwvj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gjynaljlo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtqiyyhqq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbkrmuwgo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gpitypgnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gjlycybsf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gjsyxorpw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gvzmyakmi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/girrlftho.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gjjpcivux.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/ghiygcrbg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gvgjvrnso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpbtpjkyr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gnskptiyk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gwjfhlvkv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gjosatoka.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gyqwspoqe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/grhlmxfie.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giininend.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gorbxhpxv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glgngzzif.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gawfirbme.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzjrrbipr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ggbkhfxpm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gimiqoxyp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpljcerir.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkoxfxvvt.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/ghjsndlda.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdvwqoldz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpvyvzzan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpkecfchx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtrqwnlrp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhrdpey.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwituiy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtgtqqybo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/ggslosmfv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/genwcxhkh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/ghhixhtav.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/geusvoigk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gspionmiy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gmucirxtf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gyuburgfd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gbpkimfgd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gvdiuviwo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gctptkxui.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gbrrlihxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gprdybjfb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gxnbypsho.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gmlpoqvqv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gtbwavmny.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gznvrbxkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gektnypbf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gozszzssw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gnkvtkprx.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gvgkusjib.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdikrmbdz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gelgqwaes.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/ghyxyzuas.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gqpjrrfub.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvepnxfef.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gblzwooso.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gojknefdv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gcphpxfbb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gekkwdnvs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkystsuhl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqbvyjncg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gapigbqdj.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gubqqnxpq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gnotwznud.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghrrqhmkv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghtvbvtgc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxghxtnrc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gvfabnewo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmraxrgzy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gzeaksrnb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghbdtkkdg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkjtzfutv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gdmobnxfq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ggbicwltd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gshtovkpi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/ggrorlggy.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/goykbfdef.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ghgakbpwk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gnlfaacpe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gclgfnqwx.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gwmrcurfj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ggiwwidlv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gryvdowrj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gslzbvbyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gguimrzsv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/govobzmxr.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gbacxbwno.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gliyuernn.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gunamzxgs.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gpgkrdkye.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/geazcgnzv.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gemnifayl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbloianz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gufviskxp.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/givpdtpfr.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gjnrxaqcq.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkdzckgkj.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gheuewzjk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gljeqsjho.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvpuahrbm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqbvbqfw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnitwgnue.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gcndtweok.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gkeluwcjs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gsnphgqaa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gjtntmjlp.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gweafider.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gohykfxki.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gchbuwmtj.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gnfmedznq.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gyucshnhf.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdknsmqyv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gpqwyrnni.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gtqtmpuiw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gzjsujlsd.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gsahdnqow.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gcsyjxqwl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gzthgbwqu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnjuhtnqg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gftiwyjjx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqqskuagk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqdgdmdgt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/geflpkmeu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gzanfvljg.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gmbfsmdbt.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gbvdvgukd.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggjiozlta.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxmlfgztr.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghaxzspra.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gagpdeptq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gycyrbyid.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/glbpwzkow.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gtoazjsag.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/glunfhaiq.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gsiqaebku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqjfzgwvv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gesrxwswp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/glckrphbz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ggnamlitu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/grzbihxsk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gaaexyfvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/grdrloqon.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gcqmkxjpm.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gaepaawoq.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghnlylryi.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/guuexirdt.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkeuzskib.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfqcsxavv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gbnlsemrr.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gzbozlcsi.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/ghkrkdvll.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghmzhdmoj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gnspbwjuy.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gsscyebni.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gibiatmwd.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gkkgkortf.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gdbozjeqj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gquvrgazf.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gdgfrpagq.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gwiqkjnpn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/ghgmbhpcd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gresvmalw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/ggbmtsudp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/grmrciqve.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/goedavxye.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gxoxrtpyw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gimvarrrx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gasiagjyy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgpevfzt.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/genaemtel.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gypvzbtyt.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gbxkveypa.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gkzlqksry.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gpyrkbcvs.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gtymzruqq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/giuajzjpi.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzpbcvxnp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gnbqqgkpq.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gqalylgnj.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gkzpcderb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdvwbxois.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gpcbklusx.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gjixxyqnf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxvtztmtc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggyajkoua.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gqjvkuwcf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gzijddnzr.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gecfrkffd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gapnuafke.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/glwlncpdg.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjkyqqplf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/goycweesu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/golznbeki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/giluortxk.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjziwaqcr.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/ghbskttvk.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gsfzlxkqs.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gyloenkbh.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gszjiahzs.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gzbwywfbk.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/guimwvkcd.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gfgytneec.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gcehpqoww.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gfszorqtf.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gmarwutol.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/guuqtjfgp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gmdwadqda.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gyhuphwho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gxgrkcdct.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gxvyiisqj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/ghifdsnzi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/guczvchbo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gmsygotmd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gfgurtskp.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gnyhrzyjy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gaknffxey.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gduahdvcs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/grqnypqiw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gekwvpvtw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/ghujiertw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gycxbdwlf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gmzqlpqvy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzhkeulpn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gdggzyqao.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gmwojiawv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gqsmkndlv.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gylfeewji.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ghfrrqrpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/girurgccu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gyzizcmyo.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gyjurroww.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gxyottafu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geubmombj.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gjcpruufy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzixucnwa.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gqeyqoagr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmuheqi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gtjhzlcfz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/ggnldxpao.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gukmnguiv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gtavtdwnv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gdyezaiqm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/ghnewgehw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gnwaibgnp.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gfuprmnmr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gkrtdpqmx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geduafpdu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gujbnzjyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gcdtqdowe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpxziymoi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gclkexdbh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gvhjydaaj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gclovfnvv.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gkostbbju.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghtdgmxhy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvcbdmhzy.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gnkkxtdrj.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gtvhbnosj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gldymqpms.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gujllzxgh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gcsaqmxtz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/godcrgkkl.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gcsfkszop.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gurhntous.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gqorhdzxa.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gtgkinqdt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzaohtmlf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvwkarydc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/ghjxmmfcj.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gvxeqbyav.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgblztas.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gizlclrpa.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gfrrenaxi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gjfhgwdvc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gynklhypm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gjqhqizmu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbasmdr.sHtML


<!-- 参考信息 -->