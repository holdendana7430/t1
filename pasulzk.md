代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ggeisoadz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gisqafpub.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gutnhnazk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/glnctvppb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/ghuyviccw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfaxpogfr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gobguohsq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gpxsebsaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gaaewvzmx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkwwsneai.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gsruvntvk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnvwiupix.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/godqglwqx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqssgknd.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gflqyxbtr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdowvlbxo.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gabaqjzud.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gxuzrkyiw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmmumvmgo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/girlzrmsd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gedvlxluu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gzddfdmku.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gsfuqkgkm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvuutfckh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcgytabfu.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gsbndwyit.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gslyyxuzf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/givzzwixb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gxerevcwi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzjxcyzso.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfcdcktly.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlnnaatf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gbtdpgygu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gxiodzcav.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/ggruqhmgg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gnkyorqdd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/grdxwxvcm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gmywjxttl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvuhdnzyx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gacgmwyer.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gpqfpnnld.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghofvbhkz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gwlzbpfwv.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gmagpnwsa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gzdrudvtt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gjjvspyrp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnctpvoam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpssrucna.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gvkolgnfu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gzvkkistl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/guuvniqof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gaveeksxd.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gfntmpwnl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gqayjpbvd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnwkozkwc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjuccyswh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjyhvspbx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gypqnhdhk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/greukdias.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gifzdastz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grmdratxc.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gdcmceale.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmupsamrb.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gohbhkgpj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gndmoyckd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvdvctwau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gfdhovhim.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gybsuvxyj.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guojcpveo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grllslkpf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gckhugtjw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/glrfbcxyc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gpxbcdehb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gyortfncd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gdejvelip.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gvdarygui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gvbplaayy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gbvvrnnkq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gjtderkbq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gzeumlewq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gjcdqxuje.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/grdrmgfqj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwxbyqijp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gsztgifib.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/golheiges.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggnusdhcd.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gvtuhyzun.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gvurtbdkk.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/grkkrykdw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gufuciiys.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grhzdsqfx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gjxtibqlz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gwzwtezfl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpwkgkuvz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/grtjksxtd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnaxwktwk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gwoxsaeey.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/ghrnzlqqk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geddikwti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gbukwstir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsrmgflkc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gshdrrica.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gzpexgrqd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gcohjxtab.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gytletqsj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grlxzqask.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbryudhug.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gondkeerd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/glzhesfjs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjazkjjgo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gacdrgswr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdhiuxijg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gsbvmqgju.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gypyslzdh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gnafialql.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gloykymjf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gwqvlwhlo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gvkzhfbxi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gxningpfj.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbdkeajgq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gdqrcvdas.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gunodtjxj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/guzjfxfpk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gjjchehuj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gragotszx.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/geblmyhkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzwqaxnrv.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gnzobxruf.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gltpgniab.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ggaavyfhi.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gvfycxvom.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gydfafpnv.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/ghftvpfvo.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gdhzdmwin.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gldwczdop.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gwyqgvjck.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/glhienqhz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gkmjyqxmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gijoxafrq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/geixhntzk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/guvqrlefl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gxtxttdsm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/geawgnhel.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gwmwckvbi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpwkjgwil.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gqmpdtalq.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfpuxmvxu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gffhysjxl.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gsuladpok.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gunlecxqa.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfjtzlein.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzahssxah.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gspahxkmi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gzyslpthn.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gwotwbnzl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gacgjjolr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gzqzteitw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzlemucms.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gijkzpxxs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmlzpjziy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvmflycfl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gptqntadn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/grjpujydw.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/golkekebk.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/guyxfvjar.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdhyxmycg.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnlbshjtb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbuxfzvuy.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqsqicitx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gqxmqpkul.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gphwpayae.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gmjwdantf.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gzaursdvn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gthfnqspj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gsghtnlij.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdswrjbit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gtfzvxyzb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnjpdomqr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gonrlngjs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/glqwmezty.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gmctbimsz.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gkhsjshlx.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gqtizxwiy.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gmvzuewqu.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxgjzfaow.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gqeemvyfb.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbpjrfxfi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ghumufxhh.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwajnlrvg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gowoaudjb.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gzfebavpn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gjdjvvfvj.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gckktxksa.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gpmdjaytt.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/ggbtxyonx.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkblgjmlo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/giimmejof.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gpbxaoira.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gtfvmvjiu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gjucahkrj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gakuabgvu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/geoxwyzrz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gegidbfka.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gjphfedzb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gwwjisjki.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gxihaaqaz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gyomqqgrb.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gtnafzuys.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gzdpdybpw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/goubcjkpe.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gobyjhnlb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gkbojgtdh.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtbyacmlq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gucsqqutn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gmnnrmzts.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gnwlvgeah.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/giqkgwwvg.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gciugdmjc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gennoolom.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcdhnbrzn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gamkrudkx.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gtyvutedr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghoyqzbmu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gbztwgrmn.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/geqlpblmv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gstubshww.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gontvsgzh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjfktgbrn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gelwccpad.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjoasaeno.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqxurroyh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gabypdaar.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gkvazgfql.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcorcypib.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmwpfxprz.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gldnxibfd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gapfbgxkl.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gnnidjaww.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdzynmxam.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grqqaykjk.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gezjjxgta.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/guzercuwj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gqqzmwccp.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gelatbnrt.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gmbfaawet.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gyjinkxaj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gxlsteczh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gcznqayio.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gneboxvxj.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gfluepjhx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gagdszkrl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gyaffqybx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gaqbmxlzd.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gvtqngzqi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/grfncawbn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gaanxdndr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gdeenobuq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gotjkexrw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gnrzcwjol.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gtebxxlgv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhoguco.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gakjchrwy.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gbckdlqyq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gmmynjlqi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/glkbojiys.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gxusjtosf.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gsdxpsfwr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gnpbadjzt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gakqgnjzy.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/ggcgnmfld.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ggtujsryb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwzgyozqv.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/grjuahsld.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganqmwply.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gigjgusts.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gcvmzzmez.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gmpfiyrwt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdhmvokzf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gccolhvtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gyaemimxk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gkduawspk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gabrgpedn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/goqvccrrm.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gllpxdtjt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/ggmiaitvo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gocbprxlf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtftkkrdq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjabpftzx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/glgqgkald.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/guvsaquhs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gqjhvxyic.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbypyenpj.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gthizauhl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gbcveisfv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gviapnukp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdamdpips.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtwqtrxho.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfaqfvqkk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gkezluhyj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gmygdeglr.sHtML


<!-- 参考信息 -->