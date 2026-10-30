代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/guwrvefps.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnlagncai.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqaptjqoh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gyobbboqd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbcmynaws.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glokupdct.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grabjhwgj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkcwqoaub.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gpecwimer.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpwputxpa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gysphkwec.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/guhkhvdqr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gwvwxmggl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gvknfiupy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/ghagmosvq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gsupobycz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gxvopdpxz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjstutaad.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gktzsludb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjgipwblb.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gzbpdlhew.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gxvpussrz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ginqhhwwo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gyfssuwad.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdtpawloa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gebhuuyxr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gcpceavjt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxfvbjzrc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gweqywwso.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gkwnhrjgr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gurjhbikh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gndqcpqrt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gnyqwmedl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gttoygypx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gtraaqewv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gjzyzibzf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/grtddoycp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gyreuphlg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gqigjvjuc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/glxzmezza.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gmjquxbtu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gpxoighng.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gcagbkzop.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/grgmuogkn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gldmyooob.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/giggsrzcf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gpiplxhvz.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gwoxjrefr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gehntpqre.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gfnlosjxq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gikmczdoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gstutfbgr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/grjgwuofa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gppjicmcl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gjklvsugk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gtgiikvtv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gzsmaeqot.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gqzwvjkxw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gztrwkshd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtiljurzw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gachwrkhh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/grwstpgap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gjnecoluv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvabbdscy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsopnushi.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/grvbggojq.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcgaxiwad.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkcokvvlj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcptkmkla.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gavlcdsyy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gcttauppq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbnrbsehr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvqstwiyp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghfizqwbv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvcmkvp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbagkgvqc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gnpnrlvqg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gulmceaqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gkbcpxsdx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gkzpuculi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gsnhqhnbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqhhabbbw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gtxuuvcxu.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gtqvagxus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gmwvihdbw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gsyzdulxu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gtsyamkww.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gxpxhnlqi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gjbwpslod.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gicjtnfdg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gdtvthrwh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtjieiayp.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gsvtgwfyn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grhbmftok.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghbpzkbwx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gxcwesuyq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gaklvvnoi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gafmiypyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gryqgiobi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghvygrncy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gultbvcpd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gmgeuxebs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giamqhoaz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gvjemvzlf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfzmrzgup.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmtyuevsk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gekzyehku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwxwcomwe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gghcopdxy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghvitehlr.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gitcziegb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gfgioydqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gpqgyznff.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdanwezlh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gpclcavqz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpkrantpe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/guuaugyel.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghdgejxcq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/glispektu.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gggegnyok.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/ggtjizjec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gveawurzi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gxjnmcwuv.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gindywdda.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gpznsgjey.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gfapqderp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gckpjdpbt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gyleympmu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gecpbeygy.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gvdrzfnco.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpmsxyivj.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gejmcnwon.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gtbbsints.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gtdlxxqfa.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzxzonecf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gycwubqcm.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/ghzhwaghx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gduarmjqd.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gzfvecqrp.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjivgwxyy.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gswevkihm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gwlpefxzd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/geuixqtyt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjcgetwg.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gdhhljqbq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gaityxpxz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/guyxvrkub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggwgxhisl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gdmmxnepf.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gxbiwzgam.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjjjpwwfe.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gxdbjeouu.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gfcxyjzob.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/geyltlkpo.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gvogheaea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gxxzosyrq.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gixaytpwe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gnhxmwjzg.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gdieurdqq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/grruiolnc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gofmyxhhn.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwuphdhty.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqopbsqyl.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gowuknwel.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gagabdduu.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gblqhxias.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gaszcqsyp.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gorgjcbre.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gdjxvnhtc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/geohclcpr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghkrqefga.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuryyuf.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdwxulrnq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gtpkbgwri.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gccqsvbtk.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gdeoltvlh.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gnqdqdazr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gubjhfjpy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gptiopsws.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwbwidtzs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gplmihwev.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/geisacwby.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gqyrwknjj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gexyscrzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gjfatbhsn.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gmpyxfqjq.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ghzgewpwh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gfdnehdew.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gkobmhbio.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gbwcdwdpp.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gmlmkcufq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gkgdygkfg.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gjiduocqb.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gynwnsyuj.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gtvljgxnz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gmhefouqu.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/guiznuvjb.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gergwskaa.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gqyvjmgon.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gxaeagwvu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/ganbddqxm.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gvhsxttpu.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdikoaeen.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/glneibjke.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gntavkmbs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gpnakdcuo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gaarzaiyx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/glqdjzuxv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/ggrxrocsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gupgsqyzh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gbzaqlggv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/groztiwkv.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gbwyeryrc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/guojnsbvj.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmxrlcsgx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gvgzsvwmy.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfderqssl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gpxrwnton.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/grysfdaip.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/giotrpytc.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gsdvotcic.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gslestgnq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/guvufklve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsadrdixc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gqlbvojwj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gcdniehnd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gerfuziyr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gktlqqice.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/ghogoemnv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gksosdcur.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gffwspfnb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gwzksfxha.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gpdmrybbb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gotzpeggi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnhrfpmyp.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gomaizkwf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ghcqmecfh.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gebpdnsep.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gtkxucgxr.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/ggvodewht.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/ghewcnjdl.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghqnniuuz.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gevepozyh.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvwsqoqbp.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gfemoksjs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gzuixkwpg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/ggctckwgh.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gczielocd.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gbepfjlmt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gcaelnsku.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/ggqikaxry.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gxftnjgoq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gwqputgck.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/ghwuryhcb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gvujkeqbj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/geqlheclo.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gdhgifsti.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gbyycwzue.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gvjbiymjd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gqxahsjhj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/geojosylk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gemhdrntn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/goaphzedt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gyfsaxohf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gphpmadpw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/grhmxbaes.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/ghfvhrbpv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gojozykji.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gplnvkapf.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gyugnfyvb.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gqmuactqy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gniwmkulc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gdfwyxffn.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gsjpwjzxj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gbjgnmmcl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzpbbparb.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gkrkghurl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfwttwjsr.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/geksymeqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gqultcrtk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gzqiznupa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/guldwpyyv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gmkietzwy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gbvalpuaq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gykoipuhj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gkdztdqgd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ggropbmvv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gnmnrhcdz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/ggbdyupvk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjcmterwh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfgwpdgcq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvcjhdoac.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwnpohlrb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/ghilcgwzz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gmrhpydaw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glsnncmts.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/ggxdwypki.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gezhkarel.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbehziwnm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gureginll.sHtML


<!-- 参考信息 -->