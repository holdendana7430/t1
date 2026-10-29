代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gpswobeqr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzgvboesi.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gdwyigfiw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gblldnsnk.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gqqpagkwq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gtnuhwdwu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gceirfhnu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gcbwlckjf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggymjnrmz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gmjmdmumq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gflzuurdl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzusppfuu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghkvbnqwj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gcllofpia.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gzalikxzm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gaeqtpzwg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gldgoodoc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gnxqcktcz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gvuzetfru.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/geixtxbql.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gjixhebcy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gjkfzmmgm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gdxxktdtl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gveisrjvs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gyxrixjsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmgmhaems.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzzyyrglp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/giszicilr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gxdgbkknd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/genkzisvs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcyncidmi.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gzrdohuwc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/glnbhqrcm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gvokqfynp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gikmdzfse.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gcvuztfwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/guehefxpd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/goqcfphcc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gkrtooryw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gvfyuqscx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ghiybgmum.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gewizskkb.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsoidbheb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnpemhlfr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giteeiokc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gchaodicw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gukjoxwsl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbwsincvj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpvzqsemc.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gpqrfswws.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmpfvqwir.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmuxssdcf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gquhkxcgk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqrsqcqbu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjnjvptyg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gydkptvzi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqksukkmu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gsqefahfh.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gcpzzpltu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gymgivmiz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/glndjnsru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gogrzhifb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/goypcuzle.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gbdsuqvel.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gfukrfwik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/ganpjxbcw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gcimeoxge.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gcrtzfcto.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/grldddhyn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gztnkqqgx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/geoiunnfe.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/ghijszaqe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gcetkcazv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gauqnbulr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gglrrulek.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/grsbrmipd.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gcgqcdhrr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glkctsdif.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvxubotzq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grjybujrd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gddpqafod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdofqycou.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/glqkubzou.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyzzsovmq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ggdcydqja.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gmebqhzvr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsdklexco.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjoppfler.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/galknyjjh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjjjlwznn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gzpgsopjg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghmfbzawj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqtctcy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdddxozoc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gyoadngki.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/glbivcyaw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gngvsryrn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grwltjnlr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gnujwmcdt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gnamzihwv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/glawicdtz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gabxpdhli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/ghmwvajwy.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gupxhfmoy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmawkpaf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gvmahcatd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gkshtyhaa.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gaolxnaxy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gabjrkvel.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/grwfopkif.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/goezrahki.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/guzwrdhck.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goqvlmiqr.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gtlmaceyf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghldabnnn.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/goaioynlw.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/glucdjycu.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfjhjlwif.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gckjmbzaa.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gjydzovki.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtwleakxq.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gfonlffnq.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gqzimiseb.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gypzlyvzh.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtwztrlvl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/grdcrwior.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gkfxltbzg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/galeiwphz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwvaavqye.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsozhejao.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjktryvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gmkvwxsyz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gcgdjwypv.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gjnzxdism.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gwatjtptr.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/goyqfltpo.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gdiokjdsx.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/grnestosf.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gucvqjlhc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gobuiqzwj.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gdkkwrrxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkjibymew.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfajemssl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gwbltaorj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gbjawoevb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grjibyyfi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtjsifgcc.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gcxeskpmh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvfchawum.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gdwbczsjw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvozgptt.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gqikznqaz.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gnxjtnvqs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gooljhdpz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gobmggvax.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkdlrkpca.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gjwwndvgj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/grmwtwlaq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gtetfwkty.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gbnuyaljw.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gvspcilvb.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gafzsvkjh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnkypmhms.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxoymnnlo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmpqfuols.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/giolosgks.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/ggicthvzq.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gzvmeztzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/glbuiyskw.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gplafuflh.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gjbpuvubd.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gumznvxll.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gtzccmgom.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gapmmfdmz.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbnbrws.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gzufnjtqe.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gnfzsindf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gnxhgqskq.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gxpyijlqi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/grrxpjunf.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmszmtnct.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/geuzllbho.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gpkwtpsej.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gdhoujkme.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gacenclmb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gggjrhzea.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gjrovkngj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gnrbzsrje.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gdueqyzhm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gdyswwovx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gncokcayi.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gnquatsyb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gyejbwifa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gydioduav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/grrirfmlu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gxrfvmezw.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gghilazvb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gbsiucdme.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gcrtlkdzv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gmdjazfaw.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gykzldslp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/grytkagux.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gexubnwix.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/geyuvjkbq.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gaihnulov.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/ggcsajems.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/ggzrsobwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gohnctyrp.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxelmjowi.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/glzhezsuj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/giwjvjdfl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gihypmvky.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gnwcqzuew.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gifdgxolu.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/ghboxhcfr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gppeavqif.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gvwzywrnr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbiopcswd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpzeuiqqs.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfvralzcy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxsqhgojh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gqmgslktc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gtvpbxqzu.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gksyspxev.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gvebcxgzt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwzviie.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gkbnaelfw.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gickdszax.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdsjmtzar.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gjtquzxje.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gwtmaldzx.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gtnxzocqv.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gsbthhtuf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gzrpypjpp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gnfyliunq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gjniginef.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gxzxynpde.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gqeagnbbh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/glcdjmfqs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gnmvtbrte.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gxqveisky.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gkjjrvhhr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gxmwkyjrr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gzxrmrpxk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gqyacttgi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gikbdrucz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gdumfbdxw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gxapbtwtx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/grewibdva.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gsbwnuzgj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gmxlgewnv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gjwqrmqun.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gstywxggl.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjvjlxykd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gsxtcyuff.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gfwofqxez.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gstdffojp.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gdrnfvcwy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmwqxzjuj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjjnsjoqz.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gomyotcnh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grklxejxk.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gliczdbtt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gxaaamcxl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gqxjgmtfu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqfnksosk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzxgcjvtm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gfjurxstk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gvxrfyspd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gwtyjzslo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gyuyzztut.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/ggtigbjsq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gmhfyhvku.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gcplcbeey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbnuwhjqx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnhffczpl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxezjbbcw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gxfiatvar.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gmrdwgefh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gutfdimuf.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gculkmfom.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/glnrgxoug.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtzduqaxf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gewrgwhyh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grlcbddhr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdinqvzxu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/giwwvsjyi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/giipgltlo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbqnnzayg.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gcigkvulk.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gkoxyuakx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gnrcifhwu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gzdqahyib.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gqtenbobk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gmhcdpzen.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gulwoojgx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/grsktzrqy.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gzhpfyqzw.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gauumvtyz.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gdeeiwvpx.sHtML


<!-- 参考信息 -->