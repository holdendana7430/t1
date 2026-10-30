代发 wailian999

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gwnudxsed.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/geqksufdq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/grocdriiv.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/grxxhdzyl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gdhhkdnhb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzvtkxxpt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gnteyfgjx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyzglvhru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ggmzhhdkx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gucqgbfgn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjqgeamoe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ghcxghspi.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gxkuupzke.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gforodbqn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gpxlielup.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gkyyjfpsx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gillomtrk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/giaivipyt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gxhlaarzy.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzmqqilry.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gmgaqkeze.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkaaeiegy.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gvgyavxhe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghtquuiqp.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gktyegmnt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gvlvubteb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfgsustax.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/goiqfsyzr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ghvbjbxdz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmuksvhji.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gnftpmaos.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gepkswxky.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzxtfrrsi.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gkbcfpxrq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gmocvxzlg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gqqczacqz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gstxlzwfj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/ggmzdhbgx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gsylejnuq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/geomvxtxo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gvzkpdopl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gvgijrytg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gswzxyqkn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvvrbdrxl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gdeaprjlh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjqgdnijj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gggtbddve.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gwurijreg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/geyzfstmm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/ggejqckxe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gsmodtihi.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gjwhaztla.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gmljseulm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gmsjzvgsz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gilokjrfs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/grpnuqftd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gfgfxfurj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/ghilejhzo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/ghzboqacv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gqbavbysj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdsxgvzqm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gxmjsyngd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdfgvqahb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqfqybipm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gednwszno.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjvdaxdqm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gwzytiyhr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvvwbimyb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gktjjnyjx.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gccurxxol.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmxxzqllo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gicwwgsnf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gegovcxum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmczkcnbe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gzqdcbkdx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaufjrezb.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaputjhoj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggjflczbj.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gjedhdxcm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/ggwbjrfpj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gumkhlgtk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gmyrectsq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmqnmecjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gazitthfp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/grbqltnbv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gyylrpfaq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gyselfuzy.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gelzcetgn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gtvhrgouy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gmyssbfql.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfjzazaff.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gclzdmmfx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gjetqpknm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gcjeokpfx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzifkmsaw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gjwhxsvwj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gbsypqrrx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggqqkliup.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gujsyismh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkvszreuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gtwmteiox.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/glsifwpqn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/ggmrrgici.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmgezsudi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gnkmgusmp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gjujrikwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtziyjctx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkmpfcpuw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gitrqhvaw.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtdptlljj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gfwvorwaw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfrhhavay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvhjejbpl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guiicleoi.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gbcwkzxhm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghdxqjidd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gbkfffyuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gybolxkxk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gttpnqfce.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmkfslozt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gfkydfxih.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/grdnizlnw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gruqtbikm.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gwwethrnu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gtedpwnwv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gfbbntjpt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ghvrvzxeq.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gwxocitpk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gapidmokm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gysxrcoid.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gfzkqfzdi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gkbunuleo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbdicuk.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gatdkbndr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkucrmzry.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gcetknlfa.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/glullfinc.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjamnfckk.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/geimjuydt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gxklafutd.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/griycgwjf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gmulqmscf.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gyjxdrele.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/goubvjvmw.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gtvjyvepc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gudgfsttc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gsqkzjmfj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzafdjsfb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdvyzpd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbbqdedsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gggfgotnh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gfgvfrssy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/ghtmsjion.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/grusjjjvn.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gctcdbodu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gshjmmjlo.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/giuebmrgj.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gdfxfuwqn.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gqjaqzafk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gpkeiqlry.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkzssehuw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gxurwioqa.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gwvjiouse.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ggdpifyjl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gugmdljes.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjvelhues.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggswuiiui.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqyosjhlu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkfirkvre.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ggjrpkxug.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/grozinjuh.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gbqmdojxr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/grcxzltre.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzagbboug.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfhdfksir.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gicjyvjur.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gykapxwqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gxarsjjaj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gygyiwebe.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdohhjgdj.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gsemmidgj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gumddktou.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdacoflez.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbtjtrouw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtycvgotf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkhddmhkj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gxbiaesnv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gdkzqgnws.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gwyygyrao.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gsicbueks.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gpvkfptun.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gvlpnexee.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjkciztex.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/grplfngpb.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwiaiilsc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/giskyviuz.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gczaquyty.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gnjkvkuwv.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gywskypiq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gaeknjchf.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gczfneaxt.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvykrypfq.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gwftgnish.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnoiugeef.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gukjbdaur.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/guvcxtglj.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gftdbqloe.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gmnzwtggq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gffnasrtk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjmtxdkfi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gaypdvfak.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gqrqipyme.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gsiieloae.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gsenpkppc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ghbvfbsxl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpekzqqcj.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtgfvnzfi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gtkyzbxts.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghzlofmgu.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gcdnomnam.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gunvilwos.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/grljhlumx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gcnidyfbz.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gagkknnyb.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gblljcbcv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gxwugrkfz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gmohrxewv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gidwtckuv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzaibmgjt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqshdkdbq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfqblflck.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwbdjdgap.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gfemsrczb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gsmpbzwsh.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gvudyjpqt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvontaamj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ggdyfyyjw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guwodikgd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gmgwkazgf.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gsmlqvcxf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ginjvykmy.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gbcptjlzv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gibeffmey.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gwlfrswys.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gqiwufqxw.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/govswsyag.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gizcgpvzw.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gewoaoypg.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjquhjrzz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gznapovbi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/ghzrasueu.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gggzmrzts.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gpbldwyoh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gdwjbvxep.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gdbmvfxvs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gxjwclwhi.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gauzgohoc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gqagijaio.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gajpcrmlx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gsxzokmkx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gcnpgdvkp.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gukzrxtqg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/guwfkpduw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gbywrhudj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gbkalituo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/ggpyyxmbb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gyeznfupy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/ghexgbdln.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gsirieicv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gannysosk.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gfcytalht.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gtfktyilw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gvotzjxgr.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gbroxnivm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gkheumzsl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gnmuioirr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gkhvdlekq.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/ghgwclosx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gmusbatjw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdkfbyeqp.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbqoisyqe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gspcqzsaf.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gueiyyilt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gzizamxcu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gfuuxuklk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gozalsvzb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gzlftnvlz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gnrziaaiu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gsynjbvuf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gkkdqtwfg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ggmhnphew.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/grjctxiud.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/grcpocesb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggvmkkyel.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtuxsmkyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxtstfwtd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfsmartvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gbziwkwjx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gbzlwicau.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpeziwimw.sHtML


<!-- 参考信息 -->