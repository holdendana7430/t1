代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqefkgbrx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gvapdoysh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjrxuhhcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxmqnclqp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/ghcldfgje.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gjklfjjcq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gydmvlrlj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/goppnubnh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfvmfokuv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gxxkmajeh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gagrpenul.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsuskddvr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gibulnccz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphkjebvi.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gvmopvtqz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guvhxvyrg.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gxzhjbcre.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gbcwmaxok.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdyxsltem.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gbezyqdtd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfchzuc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbrbsnnas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gaxsqmsub.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrbnvlsl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/glvxpwifg.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gtoxoojko.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/glaubgxgg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvtipgwwt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gertxdyge.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gopbuajxv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gqcwkjfgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gypckbmhf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gsiziyeea.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gflnxqzgh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gsunvwemr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gbpfuxkaa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grwenasos.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gdxtokoox.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxkieyghu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gdbgxgksm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gthzfsfzv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gwnohtcyd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gshlqlqyf.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gykvdezjc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gjlcwzkxs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gjzdfwqcz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gmdcqlndk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gfeyfvguo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gbjybqipb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjdomygee.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/grndlmyru.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gcehqbyfx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwcclhtil.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/ghrcpikln.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmqxekzrr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxfamcemp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcdnqetby.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/guphihsvz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gkxiarsvv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvjuddgrx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gytvwkrkg.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gflsdhzse.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtpkbgljm.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvuplxane.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gofijvfsz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwdtfuiwt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gbwiblmov.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcardqczv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxznrodxs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggzmdmmey.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gtdqezeec.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gixocengk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdwtkpmgk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gzfrxcgbg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gynayeamv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gkmimzcmk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gpghbyfvc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gzjtdjvxz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gbibkanph.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/ggkflvhcw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gwyywsfwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gopzjohjb.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/giwhkfgqu.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gfwsegcvv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqireznco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gxrxcycll.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gawocfzaw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gmngjxauf.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/galrjtacv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkfgqblcu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnkeajwux.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gngoaxzrr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfgzcugjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/goyudoqgz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gzuiwojiw.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gslwavmpz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gyhlrfjxq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gxnydalqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbrkfrbed.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gdcwyvzkq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxponloyd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grnnavhct.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gtqhebbgy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gekymollx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnmlwlbzd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsueokidf.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gkqbnvvhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gucoyqobg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdxpqolum.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtunxfbow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gicflctxf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gmyvjyfzb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gbnrbessk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwguvvwvw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gpzhkkoey.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gfewdiymd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdrbirpe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gfopiowrd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gslcykwnm.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/grhfoenzc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gjzsfqauz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gjtmvkmae.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/govvtrudy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gkbiorwwc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbrmichrx.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gtfvmdogz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdviayhvp.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/ghmvbmvft.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gtlvbynly.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/ginfqjnbp.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gfgpmpwkj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/glcuuwklt.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gesiuvapn.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gacsfnyli.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gachxuzte.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/glmmpdsfj.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/geuyvhtax.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gfspeedpv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghjvbweyu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtfmggjcx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gqamcemzk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gsmceycje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gxaekxvcs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gkgezxzeq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gitdcjfds.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gehkroyoc.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gffzvwslr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gijpbcppl.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gsqcoqufd.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ggcahvgao.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/geeaifzwi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbuvxdzph.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gumhxesll.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gwtjlfqyq.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gtuyxnzyh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gsqursbhe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbrnlsokp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghmbtyyfs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gwobrokhq.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkjgirbyf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gjoywpulr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjktcmyed.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gdvdyurqt.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gtffgqoki.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gutyilozg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfdneifcz.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gezgbitpf.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxrmibzyd.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggvxqigqa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggscpqvzw.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gtdypbuus.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gjzxgncbx.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gvzehbazm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gcalalxni.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gaciviwtd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxkrbefg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbtarrila.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gaammpqvh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gvltmrglc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/giclwqvkz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gcrduxkoj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/guwfqygrv.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gdfconwhv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/grvbbwdlb.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdourax.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/geohsrugz.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwgxjfyvj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/grqujonod.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gludtvufa.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gtpimetun.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gbsnwyugs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gybbblwbs.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gpklvqozu.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gnnqqecdz.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gyngszrtz.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gyssjfgsu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gpvbxaqta.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gynymrodt.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gbjrkhbrp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gugfxhuyj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gdktfkvku.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gdriktanx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gmwxlfzsa.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gapbyrnam.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gouibznop.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gixqjfamg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gpuofzzid.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gtctfadko.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/glghohmni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gckpocnnb.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjasiudzq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gjoeqfdcs.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwodzmdhr.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gwbzfcznd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/glubqegrd.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdgmsxksb.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gsxyerxci.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gszidlezu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gtldddtzs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/geesmmnsz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfzdwedyn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/grbnxhoxc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpjsuctti.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqmosxpvp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gipfhxcvl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gccqtqbje.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/guybwvfut.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gytnecvww.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsuzdrpao.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqfgqdfyv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gkoimxirt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gczdqxjqh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gghcwyuvz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gaeyilwgw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gmjezhkoi.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gyiejaziq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gmlgysylb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gevlhvzaj.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzbcxsigu.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/galaqhmqi.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxqtcyhil.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gxzbifyor.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/getfijjyq.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gostfyjid.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gfpakabxi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gkytnowkt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgoooqx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gqufjcohx.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gcsmlapaq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gyrbuvnur.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gekqdcvxw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gwkykslbo.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gandqajhq.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/ghesnzkws.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gwqtlolst.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gswaczbua.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/ggetwgxlz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gwnclbuxp.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gzabnexli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuswwew.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gxoeghtlp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggrjmsamo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/giufcdvoy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gmptinkms.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gynaazjzn.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzcrswzua.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/geqdmadok.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gvtfyzctw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gkvgnetrd.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gwtqznwzk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gcklpvuhr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvzurzmdc.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gexhoqvnj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzpriaaic.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gteyugyfh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gvjswklup.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvxunajl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gkpizjgvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfnthpnlo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gwnwhbrxn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gspnuxiuw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gnsjebqko.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gmdxkvwcj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gkvvkzhuy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/giclrouno.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/grjkjjwhj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggkengpju.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfgydfaqt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghogoegjr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gsvibwknp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpihbqedo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxnguaafe.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gifxfmvta.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/guepyciha.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkpyayddb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzwyxuuwo.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gqsjgonfi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geqvuhihk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gcljslqrj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gprgctrqa.sHtML


<!-- 参考信息 -->