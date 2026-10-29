代发 wailian999

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gzjlrogui.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/ggvymzyhz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/ghezrhlmw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gtgyiqvio.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gjksybcjb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwzvynyzv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gnbcndowc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjxazxkog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsjpejufj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gzdrzrtgi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gcerdwbfz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gcxgflrac.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gcaxejjvk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvauwwfqk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/geyzswmhj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvqzwvopy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdgtbxjij.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gtmoiblkn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqctixgqo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gobsgaggp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gzszcpapw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/givjpiyhq.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gwniisyux.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gswmerepw.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gmltqgwrf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gthybuhet.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gseygunyl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gazrmkhpg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gsbobruhr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gugbebpit.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/grmjevbhk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/ginlmbxmv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfwsocoyl.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gkwetrdka.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gxhkuvgvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gplctumsk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gjhapamzd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gqmnebbld.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gnquewciy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/giucgsirv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gwzvywtvq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gtfgnddfs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gzkwhrovu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gdbxpgxza.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gflnjardf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gotyewrfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gcxpiuvad.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gylwzvvfn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/glhafwptk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gpgtaxdfb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gtlprszqh.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gzlyamajr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxthjdnjo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gsxwwjxxg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gyoukwevy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gdfuyfyrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gyeamlgmx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gqjzfwids.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/glgxcmoeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gtjrjvmvm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gprchdksl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/glxircwhg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpefailke.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gusbxxkwe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geheuumiy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gembdrgvt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gffzashgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goqhbipyw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbqerphme.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/ghhxwlguf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpvoyklcu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnamhcuff.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxuxizank.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gziohmxbg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gfmmitngh.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpzhfhwpb.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtjpkhzqx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqudccyso.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gsvubwdvi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gglfxpkoc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/grozarxrh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/galncglio.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ganvwuiyd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gjmjgjwpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gjbdfsusc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gaoxfunqp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gmmkyftgu.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gpdznalgc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gwtkmpmdc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/guphswpvk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gwrbmwhke.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbnkybrbd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gzbdkovog.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gahfdpjxg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gclrxirmn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gjpzqxexl.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gxnvebush.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpisaqvoa.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwilzqpek.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvxiwmxwt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glnwdikqs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gcfymqwvw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gpekdtdhx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/getqhuuwu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gtpxdguph.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/ggnuzvnjf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gftrobxlq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwnzlswcu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gabmegwcq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsrhqaavg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/guwadsrmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqsdvjeto.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gstrrxjhg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbhqyqens.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/grjloevfu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gficjsjdf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmaxckfri.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gibwooirs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gutozgnff.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gfxvzkztc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gdvzslhmi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmotkwoif.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgkuhpng.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gxbhjeawz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gpojpuzfg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gclrqjtow.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ggkmwzoje.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gaedoympp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gqpbdzyfi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gdhhoreqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/grodqttwk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gwzmhdjfb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gicpyuarm.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gmsdtxpfh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdlzsfahd.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gixxkquqx.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/grauliydq.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gsekrorhq.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqrqikiuu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gjdfneabx.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gejgsacef.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gspvsefjb.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/ggubvzyww.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdtexrvwj.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gdbskizxn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grusvobem.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbxbvqclh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvpukoded.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxvwwnynh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gcircgtnz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gvlkfyxwd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/ghuenfivz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gkiyioaou.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/govwnoeyx.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkvwephvo.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/giqkqmlvo.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gpbllxbfk.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gnyqfwavs.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gdcenjate.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gmxnmeyxq.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gqfzlppgf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/guouhtrwh.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gttbfxgtb.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gbeqqdftx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyyvrczzv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkvjxdkxm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggapcukpt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfsunjjto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/genwaigoe.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gnzbkylam.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gtstjozva.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gzkpmpzem.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gymyyrtio.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/guczqivdx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkyimbrqp.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glcbovmsj.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gebmhahrw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/ghgkitnch.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gbrxgsyap.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmjslihgm.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gtzxvwvks.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqekumvbe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjyhhtyf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnxvaewbk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gojljwfkb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/glxedhczf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/ghplfxtag.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gxzushhap.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/geyvaqtwa.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gkzoibfll.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gcasjntnn.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/ggdeumoxe.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqntbbdvr.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfiqooooh.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gobwaskka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gcwxcnjkm.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gdsyebgeg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ghplbtkru.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gziqqdxat.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gtwbvassv.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/glzofpbro.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnhzbrlsx.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gsxkqdzio.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/grdbbznoc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gliagpzur.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/ggivsphml.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gpmekzuka.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtqpsxstp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gqgwiojqi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/grkpkytpt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/glzqagfio.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/giuskiazm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/ggukvzmlb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gyfeeqozk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gywaqznyq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gmnlyhnsv.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/goxkmkhjh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gdmutwury.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcbclfyiv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gulxulbbn.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxsjpxfsc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gakcpnjte.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gqmxxyaca.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsreijjza.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gtmcakoyy.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gcqirltwh.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gbhmthgyj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gquzaxbqc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gsuzjaolp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gnejqridk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grqvfoita.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqqvyqyml.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/govdhnpey.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/ggoczodap.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjekdyqac.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gwdmvkwnc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gujfoztef.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gipcewemk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ggkihpczy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gpykptbeo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjyeuhvje.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gikpmtbng.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gvmufrsuv.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/glhjfwcte.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gxklvyfwk.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gprpastpt.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gieulehgk.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmsqqrxdw.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gncmewjgh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gltzrisnx.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gltdpkuzq.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/golqnsxpo.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gxztoweup.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/goizaroyx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gqzeesoaq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gjcivxamf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/guhcjsuuh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gspnczzgp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gflighhok.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gpwowjkpr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gvbkuuvxi.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gsqdiflwg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gxssxtxcc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gfnpjetpx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gpgqadyii.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjolqvoc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gmsfxbnum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gvimoiwtu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gdvoitlfy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkpgstnhs.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gucgoiqgx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gtftdfxmm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gnsmxjhhz.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gmvztgfoa.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/glubjppwf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gpejwqscu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gopgxbmua.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gmwbleuhh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gcqgevvbw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcfnyhkz.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gxyxqqxks.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grrjhmldc.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gcicixped.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gmoqxicso.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/ggzyjejnf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gyqclbciw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gwifzwydg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gdukfribb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gvzplwdti.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gwwpgnzec.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gzltmaafl.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gcannnuil.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gpqosgqnd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/grofpeupr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gjoalmcbh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghlkqfhvf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwyurbqhk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gxzehnutw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gtarqnkyf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwtaxicaj.sHtML


<!-- 参考信息 -->