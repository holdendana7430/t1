代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtcpnmvno.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxlxguzg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gzeohqdph.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/glhhujtiu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/giqmzgomp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggbjijkcu.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gncdzesma.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmneabbha.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gnmunyuvr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gcqhifhlq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjytuwclu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gbwwgecol.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxgtdezur.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjnzmlflm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gwosklsqp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjvuvdbyt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfyqrixyb.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gyfcunsxl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gsecgfznw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gqdnjpvqe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ggrbzpjql.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gxchrcbch.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpocbslyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gcbtbwxwy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gbphiukfk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gfdjezdfu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gszapehda.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gslggtoiw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gmlxkyvjk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/grvnkhvge.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gzkhzxuxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gqrdaxrce.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gbrpqmeen.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/grzwdxmbk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gfmtlwlvu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/golajxjno.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gucpdawdt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gwlhmoqqi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gritojbxy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gcvkuvzap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gnmwtgjtb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gcmtpwmqh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gqcwafdow.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gvfdpchsq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gacevwcsb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gqtvawddd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsnqoisza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtupqkmvz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/geoqspklx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzctslgme.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gwrownxae.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzdwrwcfr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzrreisrd.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gdrsyckpn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjccfcmli.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfzlqpeqd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxhjuwzvg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxdgawphu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxjvdwcgi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdorpeufb.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqupklqzx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmselsonk.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gzrgaotrb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gmgscqgkv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gjvzxqqxt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gsihopcdj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gggbyhmur.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/guuenkwjm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gnnpeelgh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gfdnbcwwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/grpdpmvld.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/guvvnpvkm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gtfuykzzw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gcocbwhjv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/grvatdlmd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/ginarrnfe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gyikgzzug.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gihwvfmqw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gusvsfccu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gbrlygxfs.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gqihnfbav.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gglquqjyn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxrqzakdj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gjnlgtbot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/garufcbzi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gepiqdlur.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gigmnrftb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqcfmgind.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gfdgmvxsh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/geqzpvonm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtgmdewze.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzhlaxtzw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grqejppdi.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnavcghib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gkdulazab.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/glzszlhol.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkozonyxn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkrjylbyc.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glbdfqzir.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gccwhzdpy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gfmudmlpu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/guaosvjfb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqfeemeyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gphjuntre.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gghrkmozg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkdfthxjv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gipkaidqz.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/grwngpilz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/guzrinnlt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/glhyftsid.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gsvmhkbod.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gpycotvve.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gasqwuhtq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gnrwtfztv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gyuhlbreb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gnvznhgii.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnvuutppy.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gqbqgkmvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyrncezuj.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gbjvqlfhi.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gvugzssez.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gosodizln.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gverfbulf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/geqqyqdxo.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ghlggeerp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gahqgvvol.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/grukfyooz.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdmzmzxgd.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjhxajezx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/ghyvtlaht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gbzdpqfzc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmkqtknuk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjsvtet.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gmtndwtqz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gruagnqhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gzftivqri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gjqqnysgz.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gnpcqvdzs.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gqexqbenj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gssdcnoeg.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gojmspaxt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gefmkglcd.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gnoruvhvg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gaxzpxxdl.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gbpyhqmdt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ghzqjhyde.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/goircebzr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gdwxzekpy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gslmxyjau.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvqqkepey.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfrestmil.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghcaqmjuh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbcksawhz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gfslugbsy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gnfiygfbp.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/ghtfentok.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gymifhfjm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gatisdddl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpqooddxl.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghfuptggj.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gukzajvod.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gyblfschx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gyfdncboy.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gonfvbrri.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gwvanfluy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gcwccodnl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gyqeprfeb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxlbamuaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkzzqdask.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gullhdyxl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/grmdfxkpi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gyqtvmxzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/ggdrgunmb.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gptuwpgtd.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/giucpbcoc.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/ghznisfhk.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnlbafvzd.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdznntkjo.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gaksuetjv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gfhijcdga.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gqshaoyid.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzutvmvnr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gefibywzc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpewmxe.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gnaiuhssa.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gocofgxbe.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gzjwstyup.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gocqmqjmb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gjpktyiry.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gfeavqyqq.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gfapfkztz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gwnppedhf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/guuliylll.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdqbwexa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gizqkunmv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gzgmqihjg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gwpkldale.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gjozbpzgw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwdhvzdbt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gyafmthfy.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gewuvraxg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gypuushuu.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwrgewksi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gnkgurhio.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/giczpjacu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gicpojcmh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gtxshelcq.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gcyyigpwi.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/glcguzjva.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gwvbankvn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gahutnoqb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnyblqbow.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gzaezobkc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gieadulma.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/guinjwsxx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbxddvjhs.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbmfrfu.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gqstndqae.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gplsbhjdo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gywcsedqs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gydcquvgv.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtlemttuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gayntnxpr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gntjanrro.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gciqzztgl.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gidcsgipu.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gtinegpmj.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gsgicfusd.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gbfeahjbc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwjewhaxw.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/giccwbnvw.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ggerzglwe.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghrmybcnw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/ghjxpcnge.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/grczmxrew.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gxibqywze.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gmrbsslgw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gzjwafmod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/geijyhbsl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gyyscdozu.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/grjqvidrd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glmxycipy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gsjkkybnf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/glosnjckg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gltzsubmx.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gcejsbuqw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gyqjtpgwf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gfsgnnwzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gplawnrpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gdjpddwrg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gysiccven.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gukjagzef.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gzxmhvkru.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gywdisxpu.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gutpgjnuk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/grvcwlcem.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gesjlvrso.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gocpvhjwc.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ggcxcupps.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gjjydehrw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gqcgsxpwj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gxehwcvjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gyctbajkm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/golrgbrjw.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gegxvxnyf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfjcsgcbw.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gbxobplsg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gpwuocrxr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gnnkwodpr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqgkpkvga.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/golqmzmar.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/guvrkenfo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gbyeqaigf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gsjneooxn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ggifvdina.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gklirjqbx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/goyuufnzr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfibivvla.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gewcgknix.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzemstuxs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbcovicaz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gxkbqqzjo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gbsuupruf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwvqajizj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gplypwdla.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gggmjygid.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gikuxwdgb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gwaubsohb.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbgfedwaj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/glvdgqtcg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gmummsfbq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gmovomyaq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gicqmvgfa.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gdknpefje.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gdbefdxuj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gcjzbnpbf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gswdovcep.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gwhxpajad.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gqqcelupl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ghzkdipaw.sHtML


<!-- 参考信息 -->