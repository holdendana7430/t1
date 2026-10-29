代发 wailian999

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gugrmritk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gntlqsgeu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkrrdrvht.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/grqqcylpe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/glfwsfjjg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/guqerdjih.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gdbiwinpn.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbikrdedr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsepohpjl.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gidgpjenq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gungvolxd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/glvzcmzfp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gnphgxofx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gurinpgfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gqbhhdvhf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/guismkpbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gkvdfumel.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gejemlyjm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/ghocmwmvs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gipqdaxle.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gscazbxeq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmwmzlqwr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gmgvukizm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gutyxyetl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gwldagisi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gzxedgtrc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxfokhsah.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gyiuakxkm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gjwtkzdcz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gxhsiocyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gohzywamz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggmpumnbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/glfknbqiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gypdselqy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gtnttgpne.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gzuphiabg.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gltuswwls.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gpbpninan.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqavutpos.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfbmvyxmc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzvnwdyoc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbatxtagh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gsveudlhv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsfizwyzb.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glriftjfx.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gkfqurrrs.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkawbuyjg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goxoecljj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guoxpwauj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glrsozpre.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwhvrlquw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvinloubp.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grsajccim.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gcyugbziw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/glgzqngop.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmynpxeis.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnfowjpaq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gaqgzmole.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gkbpiddpm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/ghwoqonli.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gxdgctjoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gduvjczuz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gozsqyfqp.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gfbljcxtd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gnenmyyls.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/grgoampsf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gupkakdka.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gouacplgx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gpzdzzqwa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gphiabgom.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsauqzlem.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gxozdbzij.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gdgmizerd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gblqywpvp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrnoueb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbxjsrixl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gwovnfjcu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcpjtgtbp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gpkxiditp.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwebiuybc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gzsqdwmja.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ggrhkcpza.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guvoafuqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/givjdupxb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gurthdtxm.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/grqpbppvn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gyhtlqfcf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grfymumfy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyhzundvc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmjkeimhh.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/grhwmtopf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gsdrddtlz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/grhkkwbqk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/grmsefxgh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbtazweol.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gubsxxbfi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ggtqrwqkk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdyalkcfn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/guezgezxk.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/giyjrgggz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gogcuueod.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gymdptdks.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gpeznitoa.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gxcwdhpnu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/ghewqajoz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gswipbubv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gqlnzmkrp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gojgbmisn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkzcbirej.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gtubxsufv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gneesjdue.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gyrapuaoz.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gksfidnvf.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/grlicarur.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmkdxnugl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gduiocnef.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsysechej.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gumceusxt.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/grbdtnasm.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqirpudxo.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gxogffbos.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gvlrhzcrl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkrapjoeo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ghqzxxttu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gskfkipsf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyokwghuh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gzotovsne.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/grlhhqsgb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzpotagev.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gawaogqgw.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/ghoneztre.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gicohhxcc.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gpkyevnpj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gjsbjxvws.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gymsclgqw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gglsbrnqp.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gutyjlcju.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gsjtavqjb.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/ggxehevhz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gurymjgsc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/getqbjrbt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzuscnvec.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmvbtvwwx.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gozvgacgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gmvpjsqqh.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gvwbbdihw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gbblkuivt.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gfycjefhm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gyalfnnga.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfhucdxdx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpcalohgd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gahapfpwy.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grwtoojip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ggkzlksdm.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvskmlqzq.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gsrlznqis.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/glugdvojb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwpwnyhmn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjkisnrfl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnabeauvj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjnluxyce.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gcbhhwbiw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gicrwdjsz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gkeaiovjs.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/guhjwlmag.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/ggbprolto.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gujgzmgze.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gdkxoqqex.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/ggzrazzwn.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/ghpvshdps.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gkoqhjwvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/glrrlknzf.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gkaykrytc.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gbzvdjfcf.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gqrghffze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/ghqmcstsx.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/giieloaco.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gscsskenw.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gatqbjuja.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gxpaarndb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ggiihbaio.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/giaulgjdb.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gzohzaihe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/ghkkppysy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gcxzncxrc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gcxpxgmfd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ggouvvxxt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gjszmvixl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gaqxqbylw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gggpgwsdh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gghjfgbis.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gfariwqzw.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ghnatpqmz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gbyfywrbb.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gtizspfze.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gtusesbez.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gtqwocwgv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gcqhhokru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gkbcpfkzu.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/grwisifqp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gbskqokwq.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gesxwqtpu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gslslqmup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gabfythxm.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/grrbmtcdt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/grljvqmvc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtwxfifvy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gkkihahkd.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gjaevekfr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gcsovhkzf.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/guqfbweko.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gqrkmlrzt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggpavevpi.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbycnxrzj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjicrflnc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/geothlfbg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gudmlyrmk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gppaefkvh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gtegtbbbk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gnmtyrycg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gmmrswqhp.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gxosqpxby.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gjueuuvmz.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gslrgmhpp.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gufsenddo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gurijkutk.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gackstfht.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gbbwbkxmp.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gbbhnpvfo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gfzbopsoo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/ghrmpafpn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gllcryowj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gmtuszugr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gemthaiew.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gwfeyoxxv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gjtvcndau.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gizbxthxi.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/ggxndcrby.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gnbxgknvy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gyynefpkl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gnityimfb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gmmzumeqh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gceedtjpx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gwqpohrui.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gpowhtyba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gpnauextv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/grbmcczoi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gogmchlsk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gbphwqooc.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gdtvwlpnb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gfhumgfwj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gzwamnncr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/grqqzwaoj.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gwwjpshap.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gzlqxckfa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmcgaykfi.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gqkmkfkal.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnfseeaoj.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gwcbcmzbp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gocbvcamw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gcyxkbuha.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqutuifza.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gspgtsmnk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gdwomafav.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/ghmkaykow.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gjhbfqpgz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gwzedleyw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gsjvyuvfz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gczefzjbb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghhsaqzca.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gefliuqwl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutvfjbmv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbghgkfkk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gdasczcmh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gnhkfauho.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gifxhzfup.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gjnekxrin.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gpwvmgnbp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnmzqkkce.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/goiyqumhy.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcgqwbeer.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gsrkrpigv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gcgrqiqbx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/grmegrggo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdixyvkuh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gdqlicwpp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gnkldmcys.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gwbhturwh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gnfmzgjfv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gkltdvfck.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gdirnvjqn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gssmetbdw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gdsvctgmm.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gpsnhsfuy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gzzdrzutc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/grdcpxvpf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gixgrrefx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gymqhinru.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gerfedeow.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/goszwwzhj.sHtML


<!-- 参考信息 -->