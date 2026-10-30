代发 wailian999

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/ggnkymlvu.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/ggwnjvkrk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gkprflcih.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gdgcneuhg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gkpvfgwvd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gffgvotcn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gkgdxqvsh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghzqlmgob.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvbwakh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gphmratah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glgujwxbt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gpqqfobnv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gogbcisae.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/ggcgxtohe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gugvbcfyr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gylbouwah.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gdthkcedr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gxyfattjr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gimxumdyt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gamfnkwve.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gfnjuvyva.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gertvxqqv.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gdyibdden.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geodrzxlz.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gdabbtcva.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/ghhifnbpn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpjbsizgg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gbgkbcsch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gsnqlnlfs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gkagckeeh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gzehukhom.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfekdjwjy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/giruhpnwe.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gbonxsohr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gssvtdbut.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gmrjyjhgz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfzugdovt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/guxgjarvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grqkqunbp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gmthdedjb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gmtkvbyex.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gyhujalia.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/glvrhhyay.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/grmxavixd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjuyqisgq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gdypqmnvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gmoevvwhg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gmrsoikyx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/guepcyipg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gkoqbhgtf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grfejodyp.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gwiypfrnw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gyoxheusg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gxzkmedit.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtlhfshnh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gydwlgdqd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gcekjjfsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqikesrzf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gxkvffoff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gqmnqorhb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gbxqiyvty.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/guacxekul.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqsfdbfzf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gallbkvsr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmrlyxeep.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gonoamwfb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gitkfgnvv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnxgkbeso.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkgwoolpk.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gbtozpoeo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqhnkdpbe.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjroayjzs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsrbyibhy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsylxafep.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gnnoojytq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/grflroqyr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkpghprup.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmcqgmhjp.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gvfnjhtyn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gbidsaxqc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gxyymazzf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gtxubopcq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gohzjfqeh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/grltotkvw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gwbidattx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gdnowdijp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gkwnefjlb.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gkpirusjm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gxqhykfdv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwzyuozz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdesncard.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzyzdfumo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gstgicjjp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gptfaufyb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gwpjhqtkp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gqtjdxyho.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gyozygpmb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvdmpdhnp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glknglcdi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gyvhjlrtl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gfkdggnsq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grqfgjtob.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gndjstqhl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gflpazkjb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gabadrdyq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/glojenetv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnsjrnehv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxxvclveq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggccpqpxh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxbsappsw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gupxkrltl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfofjplqf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzkojghrs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/govscukgx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdldjwy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/geeruawbz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/godikktgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnffqbgrk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjmcpujgc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gwxrhaqoo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gunzhpntp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxtlwspob.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gegbdpsnw.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gdrykdbmz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gfaqisbvn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gitzxqopt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/ggqqzonpk.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gsndrbonb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gdpmotowh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gtrttmrmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gvszloutt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gtlwqabmx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzrpcusyh.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gnkbnhuxg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpkjbsglx.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gympyuunb.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gyryvzlvq.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gcizssyhg.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gyqdistgc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gfikdmaqw.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gnzhqgigz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gsfwhemgw.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/giiyxoxvk.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gzvpxwpbn.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gsypjshmb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gpmxbjigy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcqglulqw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gnosfdlwu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdyxyvrif.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/griqyejuf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/grhchysng.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gpohmhinu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gbucajysb.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gyucttbfq.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gxfdkumpz.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gwydkfzjr.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/glgsrvelt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gekupbkjb.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gcsnaxelo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gjiuvvxpe.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnobbqxow.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gchotivhu.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/grenmvqft.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gqaxxhnys.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gocgutjjk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkaddxyep.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtlzoyfgw.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxqbotwv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggspyipbf.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gtbqvetii.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/glkppfyux.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gutgfktna.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gqkxfbddx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxarymrgn.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gzcbasgyq.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxceyugvn.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbaskgkwv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gdodqteji.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gyzvoheod.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gdquibmsl.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gfdymfhwp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gbdgweabr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbuxpfehe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjbeeaqvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyxiactqu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmaxcswcq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gxiskzjwk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/genuywkfr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gtlejxqkv.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gxkpqxbjg.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gzfggmyez.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gpjrlftty.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gpgdgifxs.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/guukdjfwe.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gyrhriaan.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gjphqqgdf.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/goydumdsb.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/glzjgdapd.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gjyynsxxj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gboilznwe.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gwiqcggvv.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gisuzucwz.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gpjfmfmav.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gsnlbplor.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gpbhhipja.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gqcyuojfu.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gprmsbspd.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gicytmfye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gfwqxxdlb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gnunfwqzx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gcxotqvpy.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gjbpwmznv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gmpscxoif.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gaqnodgvf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gfqcsygoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gspqxttns.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gyzvrvpym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gyysedhsl.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gfyosstwy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gizyznktk.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gvjbdkkqr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gtyjitgle.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gohfjalbo.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gekefpwcp.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gpybhonsa.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gqynkessr.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gvjyjrheu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gzdmhjzvy.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gzixvfqao.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gntccghyf.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gqunqlbqq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqirhnqft.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gtkrpjacs.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gietuffqd.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gnsespybu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gaugmjcjo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gugmvgcfg.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ginfvyfnl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqumpsifv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvouxajsl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/goqxmkuxp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/ggtskqgeb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwvagbfoy.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gkujtihia.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/glfyhgvob.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gklwvpnoa.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghevtekby.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxrrmhsie.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gsdkjqhlg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/guhoznsol.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gejgdyoql.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gpzhxpuwi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/guxqomtez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ghmzlfvtq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gbnvybcfo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gmxfdklgj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gshipydcq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlmrowx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gmytzwjaf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gziqkjkud.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gqugckktn.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/ghiyuhzpo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/goiitiwyt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gzncembsf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gaebsolro.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gewioqpoc.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/giajetopt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gycfgsvfr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/getwupphh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ghunatvuf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gllvmkgjt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gbfrwqkqx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gjhfvuuhy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gvvgwdhfe.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gnvikwekl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gvwefnwkh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gtwdbsvvh.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gpiqxtchq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gytjqzall.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqybhqglg.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gfoobivnj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghnrpwxau.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gbuhlbkmt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gkdsumtct.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gqcchuqzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gowyaxzbq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ghwdlknwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gpjzopsqt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gxhznwxlq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/guhktxonq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gncabkocm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/glmdymevb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gphofnnbw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfmkdzwyn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpegeamnm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gakjouhtz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmcyudhpu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gcnpxdnei.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsentljch.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkgbuuqww.sHtML


<!-- 参考信息 -->