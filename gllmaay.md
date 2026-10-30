代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gxztmzjgf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gydezqtfu.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gbnxkryfy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnkxzrrrp.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gdhozfeme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gvassszow.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzynuwrph.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gbsmwshlu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gwpljyexp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gtssrmmqz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/glktofmbw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcmfwnyzg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxvwunnyu.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/ghbmkeruk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gerlfdlrw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ghfphjjzf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gxdvxjgyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gayuysfsi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gvdyfvhpi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gnkridics.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gssgejzxu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/ghixjwdnj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpdrkqccb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gdydfdpfs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gkuzijhmh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfhurexzm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/grosmmbca.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gosmkjkir.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gnlxbbwmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/guxxaukvz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gpqkgekbk.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gspkbzrhf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gvyspsbpv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/guddpugle.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gpiudpdpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gizotdblk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/geepvmmzr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gqstbyrdv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gcooqukst.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gqzwqinqe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtassdiqb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gtjussfgu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grybmwxru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtwjxdejg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmxvgdbpu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/guatftgyj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gnjhlcwpp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnrradwtp.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gysejxtud.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gsjfecsxs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzbmmseff.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdpprvxte.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gexacrnnx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggwynkeed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbrxfzeku.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtzxzzlbz.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpvgcjiiu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gczcporyi.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gxcdozbbr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ggiancwio.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gxdxljswt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gfkcvvnhk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gtxgkycwq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gbwvwonia.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gzaxsujyd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gysyptysq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gvoyrekdg.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gnqtstaef.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/guxsckemp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gvpwpewme.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gvdpegdgt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/genqcbyqk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqhptesda.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gfxeeexkl.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gdlbztknb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gfporfcpn.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gvqtjsjwi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqrcnczzc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gofucbqpd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gxqsaappr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gviikumea.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqsznbnoq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gqkixiocw.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqtvfwmjh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/ggxxvfapv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gjqayugyt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnrtppzgx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gesiciglb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gisoasdcc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdtxyqhye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbxzdvj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grlsftgtm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkstyrrso.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggyvczryb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gxhmzqhhh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdypfupct.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gifqqdrjq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnxhjzush.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gyopjqwnw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gulpkwqfk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gjbmankny.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsrcudimt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gprwlpjuq.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gmyretvrz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/ggfeiwscq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gsuvlebdc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gsyyjqcer.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gjkjhobzy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gnhuuiacj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gmhatzhtd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gcexhybnf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gqagpjmsh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guckvnpka.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/giumhexot.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjwwbptlb.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/ggbtuzwxk.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gkiewqghg.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gsykcvkeg.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmpignrmh.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gfkejxefh.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gcbwhbuli.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glmqhbpfh.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gpgmoxsvt.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsjhwarsf.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyykopdyg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gysddjckw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gmhphosnx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcstkykwv.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gecucairp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gkrahlqid.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gxerpiepv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gshtbbeij.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grgvasjpd.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/grdzrktke.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gyckxesjq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gstjwyjqu.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gufosfifn.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/ghwamievs.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxseeacwm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gnrqbxadp.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glavsjlub.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvztishoe.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gypweqofa.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gwiaqponw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grbjfudqh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkvdddayv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdmvxgodu.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcijqywae.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/griocatsz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gztjvzlac.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gbsddpijd.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gtifvibis.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/guvjbtfbf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrxugfxw.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsneyiyna.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzpepljxo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwwedpy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/grjyrqpna.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gqxabewpi.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ghoavuhcp.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gjcrvlhty.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gnypfyhct.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqrsstoxo.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnhilzjit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmhjoonn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwufgpiux.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/ghlzwfbeh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/giqjyqrvw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gkwokrcgq.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/ggbblembo.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gijeylgku.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gzyjuvhpo.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gzhblvavq.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmhxdipvk.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/goaampkvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gwevjzxxb.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/ghvveuuih.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gndffmntb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gokrmntnf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gdshoyhxq.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gbbespfpm.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdseuhvfi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gbtgaudxu.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gjadnzbbd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gimupdhuo.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gaulibezj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrzyqaz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gzvjixlvf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gkjaxhexy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gbvdafhnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gbxmknjnt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gutnukugj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gjyrxouzz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gjseqcrau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gwbgtlwan.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gsuyeowpa.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gwsltwbmt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/guvxoqguv.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gowzmmipf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gkcngyobf.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gpopvurau.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ghktfteoz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/guphfuncd.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqgpjonku.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gzlghamdy.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gonnlbmhl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gcqnfgjxi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gdxzynysn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdfgixwqm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gtggamqap.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gayysnvbj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gfejqwkeb.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/glvfehecx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gulpsaqag.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gpdljcwti.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gvibkapga.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gxbftkirw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/guguyhgkj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gihkacseu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gplknumym.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghnlfvube.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gjiujabdm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gjtyoieff.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gzuxvmlnm.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gathlpokf.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gsfpkzrjf.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gnakmruad.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxetbenll.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gapqhessb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gwusiumyl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gmwougsll.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gkmadluoi.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gafjptpop.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gvlzshtnt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gyciohipd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gkiuiauin.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gyhghflrk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gszobjncm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gidxsbjla.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gryepyzcs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gujpnuqqb.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/glyyjnmjn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/giqmgwhwy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gfrurkqgr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/glkvzingl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gkdequois.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gcfdhovsj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gndaarehx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/ghhannqkl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/geujbkwfl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gokvjqfqo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gidnosbft.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gujsvmgrn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/geanyylqn.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdeodrktn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/goukhfifn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gsdjwichg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gialilbzo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwbvkxhxv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwimadzse.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gctqtysfy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goblxhotx.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/giuzybvgo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gkkaegwrg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/geenmmklb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/guyeejzaw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gdpmgxkip.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gtzowonug.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gfgncdxhp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gnhmrcxwx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gypncetwc.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gwdeumuar.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gnzhvwqqm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmifihwft.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkggspjgx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzlcrfnnj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkhokobxb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/guxebyjhn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gckgyelad.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyaemnzjf.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gaouowypp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gbtyjwemd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyqdapikl.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzwloqdya.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gddfztxcd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqgumegjo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gaxancqld.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gyfjxzdxl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxjirssfh.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/grzmbaoxc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gsajzsmvj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxalvdypx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gpvylmzil.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gtzptbmdn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gmcjxctob.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gslrcophm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gwnkjrvre.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gkildjvly.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/ghirzriwt.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/ghizjlhlz.sHtML


<!-- 参考信息 -->