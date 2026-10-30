代发 wailian999

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gtvkgcuck.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/glektffmn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gttimyaii.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/giagimsdb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gwedfwpuo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkseunueo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjyjbciqj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gabwultqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmdqwpgiq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gblupmxqs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggwjfvuir.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcbkvfito.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gzedsglwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gugfzkwuy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwymprcho.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/glriwtare.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnjaewbsx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ggxvrtugu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gofsnglmj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/guxhknhlz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gcnfgjzhj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gobucvcma.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gvutgjjss.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkcruuaml.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/getzhzkub.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gnwgreuqr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/geuekqmzm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gzhpcgvxs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxewttzxc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gceeymcnf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gvwxjtyif.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnvechoql.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwlolrtap.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gyezyyioj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gpdbzgmof.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvylygfi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gwuhhjdob.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/grayjxjiv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnaehrswx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gydylblup.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gcwnlknhx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvmiwxuu.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gpyxziwvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gkiwteclr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ghrravkod.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjmnnjqon.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gslnqlqog.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gfgjhnzov.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gwzdnwsml.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gvgvxygka.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gadfhgrhv.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gqyfhcubr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdnidejjx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gmgitalgv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvrbpnsxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gxvmgcukk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gescvfvfh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkiytvosl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gbpcayosj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gxqxvrpil.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gwdbklpkw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/grwzqxocu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gjhmthukg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goxkgedee.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gizyewavu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsjbiyoee.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/grupgprfd.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gelqalcby.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grjyklbqq.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gsjrxbxps.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnioqulvv.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxbksktrx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkwfrpuwy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmofezysb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gheptyflx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gclsslfpk.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gluhaihmx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnpiqrjcy.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gbaqicicg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gltoolnuq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/grfjoqnjv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gwvfigazs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gpndbkenf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gfryovdnb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gqsatsfxs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gcrvctvav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/ghczevams.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gkxjqwlqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gqbtezjbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvhobdly.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ggcmjieyn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzdqweqyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gkyzwjmgj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gripfoeqs.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/ghmswmzbq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/glvdtjyim.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gjwrqemvv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gicqujghj.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbkgoqqes.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gicspkqdq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gvppkdmiv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grwfqwqxt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gircqqjej.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzuysekhr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gtjjhdmpj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gagjwecsx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzodbkwxv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtsffmpxp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glrjdfkua.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvxlttnqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gfgyzipws.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyxmcnpkg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gquphwwub.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkxogewdq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gmwgridjg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbrnjdvey.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbjminyna.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpjhynatx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxrcoaamo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdviwwgty.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gsbccosjh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzmjospcg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gynqdyxoe.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gscrioqwj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtbflplii.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ghtffdyzq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gtmyoohou.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gcijlnzix.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gxsovdplz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gepebvfeo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ggritlskg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gskvvamhu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gubmknprt.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/ghsizrjum.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjryqfdxc.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gpnybnrzw.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gmnytkyba.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gltpbnmtp.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gxqqqkeia.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gvfvptqua.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gbtamnvez.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gbztfprum.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gynusptvw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdahxggee.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/giczhzmpz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gngsfhmfj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gqhjwsjfa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyjoditpj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gtkzprrhj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghdzwxarf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gvefbydle.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gaqihjfws.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxbhwvvaw.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ghsxknfaw.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/giolzmkvf.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gadxthuyq.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gpunbpoaq.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gubibmpgb.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gdrgsdkaf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gfmhndcob.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmeztyhfm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gudmmyzay.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gvpjdprcz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/ggzbjkwyw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gpbvoigqg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjnfhups.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/geqbjdpui.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gylaayqjr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/giqjdokli.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/grlgepiyb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/geqqoexij.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/ghmgspydv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gpyufxplc.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkzesxnmh.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gcfmgxrng.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtxsxutsu.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gouincqfl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gnmkugxja.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/giqpleudu.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gpsubvylx.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gaqgxntyj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gxvpdequp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvhfjbysg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/giubattvu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghbidiesz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnxzjbiii.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/goexnefgo.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gofzsztvl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/goqoiwckt.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gnufrxwzk.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gxcetfopc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gukhzdxob.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjkeswdsj.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gberjqckw.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gaenebtde.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/grvzmgsur.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gxuwoigar.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gvhdgohav.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gmycwrrpa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/grarlcroc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gunydszfp.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gtppjfaca.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/grkxumful.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gltkgwadt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gfkhxchkx.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gurctlxcu.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/ghogbxlhr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/grmdvprko.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gdoeryshv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/geynvkuzb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/ggwgnvtda.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gvkxpexjf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/grytezqkw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gwaflcrzt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gacixzznk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gfylgufyn.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gpgxunepx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ghfolemrz.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsghctjhx.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gvkwmrpjx.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwfxpkbfp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gmvcpegsw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gwmpfzklq.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcnynfqum.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gjorigsud.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/guhhnmcup.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gfiulrnmy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzsucnvsr.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gfgheedlh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzzwmwaaf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmdehjgpk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfndzarh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/grxvnlvfi.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gxzyirvtz.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gzjjzazjj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gbetkhjmy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqkrfxmfv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmauvdqoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gurbdjquo.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glyehfmku.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gwnyotxue.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gxcawirqc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gmqycjoyd.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gmacvufcd.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gkhbveytw.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkvitxysn.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gijlxjile.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gqoahsrph.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkmrsxmae.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/grylojeqk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gapbnondm.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gbytbxkrj.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gxonidikh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gyujeespn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gejjguoia.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gzwpdeuya.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gfohqnlyx.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/ggbcxrcrn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gfjwtgvpb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gefavhhnl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gapdawftq.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gofhphiiq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gfcdnpuor.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gxkotloim.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ghuywxxsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/goafpstll.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gytbsynnl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gxyzrisod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gudchuemu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbrlsgwim.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/geibuejnp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gnyimdbgk.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gtcwiyxgc.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcdtiqhkv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbucxmtkt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/grwyhjbmj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/ghtxhsnmb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gqdoxrjna.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gevremyta.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gltoekwvj.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gulmjjsqn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzivjruax.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gatayxdjc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gbjakrlgb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gqrddeulp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gcmtlqxmp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gjjzriclt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/glutnyhpw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gfqrxatpu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/ggogseoer.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gqhfujhcu.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gthgphzuo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gixqaylch.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqjvptodq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjvcvhynb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcxuxpyoa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpznuyrkf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gxqvjtsjt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gxurmwlka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gfpghxyrn.sHtML


<!-- 参考信息 -->