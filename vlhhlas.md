代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gccvixjny.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqztoovgu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gehvwdkzt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gfcjrodrg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqfqprstn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gqnynrlyo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbavdsvpi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqjprerhl.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gtdmzatci.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gpscyojud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gbidcjhya.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/ghqvxahgo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/getfcjjut.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/glioakypa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gmmckbvcg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gtouhusvu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gkgfsmmed.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwqthrmhq.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/geqqumaiy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guaueohgw.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gpeipuimy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gjownjtiv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ganzmjuay.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gudvczlmm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gkmzuqisk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcfhyodbw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gcqpxxmov.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaazvriqb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gftgrbxoo.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gzzzdyzwx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gdqeeokit.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gzfijiykt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gybkqxple.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gddwbvdhn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gbrboewtz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gqcgulplc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gdhrjmlsm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gohyotqmr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/geoibcidv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gerdsxxog.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gcmfmlxov.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gynonlqxh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtwqudceq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gaurcnbac.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gcqpreejg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnapyckzb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gqmwzduqp.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gqpltzhzz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmpnznvzw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gqbincdpj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gbxcpeopi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gkxdarokr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gmyrfchka.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gnyixqqjn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwbxdqlyp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gqzkhqgoc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gysocvrir.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gizzgnksx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gohbpeisp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggaqwvtid.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxzrqvgut.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjsmfjfzh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/ggngdpmhz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtnhsxrrl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gibtqceoz.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gpwhzrdkn.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpqnmpdkz.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gexzrbrtv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glgxvkfpu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guwqvmqng.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gyifieumf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfwscih.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggcjfpflh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxlkpfjvq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gjixzynru.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gptwiydgh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gzhkeiuet.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gvtvvflbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gtezvbjpe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ghlqowvzk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/ggusrdiue.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gfcaqpfbc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gjxcosrlm.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gsshlkblw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/grtnxzykd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/geodaupjw.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gjcdutaiu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gssanjjsj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gekjeckbo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gujerklzy.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gogwhwqze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gsudxbaig.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gbuamcnrw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghhzekwdt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghclftooa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gabqjqjuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gqehfdnhg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gomhxlila.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gfgyfjvip.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwcmmcrya.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gtzgotxcz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gjrmoyxxs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggfwbqyzl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxzfvbcka.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gihbwwwuv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcubymuyw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gyjnrqlzb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gecmtcqhn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gmygpwbsz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmhrxhqjn.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gktonfuws.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gszjbwjlf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gublucmlr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gbzxafywm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjruszwd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/glyxpkryh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gawxeswzq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gszjqeymb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gfsyjwzyd.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gcdwstncp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/glxpgvbmu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gwvglgxqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glfrbnnfe.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gsnjaqwzq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gzfwcznox.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gcjahswwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gphhceqec.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/grmazatuj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdqahppfz.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gqargsuqa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guebptvio.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/ghyswvgng.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gsslqdlfl.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/guwzwhhap.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ggrqiezip.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gdexohmfn.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwblebtpp.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gihvkvjgh.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gftzjacst.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gbufeyxuk.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxubtazeo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gqikpozct.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtabbxdyf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ghgnfwjfh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gqeufuefs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnzmtdckf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gcmsazfjm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/giplwtsbx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gulegcqhc.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/goscoozhu.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzrgxlpqz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/guhuztxyn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gyttzlpzl.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gicuifmom.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/grzwyrknu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gqdiosxdj.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gihnsiefe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/glizyilrw.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gkdsbsoht.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/glwgxziwj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gqzviueqi.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwsrxerdg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gtirusqah.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxefamlre.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gvxooryhk.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gwrdobere.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gkelirzjn.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gqnpfmjbp.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gvfivwgqy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gsydpyczi.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwdwxpwgd.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdxrtoswp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzoikskok.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/goawtslho.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gzzyltkbg.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gesjuynta.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/ggtwyvxvg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gvtrkljav.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjxjhpzpm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gxletnugj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxgcawweb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtvuwyuqv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gqfwkkuge.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/ghozqphsp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/goguennde.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gbrkytbhh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gicohkyxr.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gdxpodfvr.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdutujicr.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gtsidrdsw.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gaeyqfbuu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/goikjecti.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gabyplmzc.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gkwiwuehh.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/getxnbzib.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gdtljcaaq.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/grklxwcwa.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gozplijnm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/goqpvpkal.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gnqvmbymb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/geomvyflb.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gguqrvxoh.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gnxowqpoa.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/giypnyfol.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gdpnbgasv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/guwlqcksx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gszcpsmdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/ggfjpsfai.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/guhbvffyc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gzdgcspmy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gyuokggae.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/grpmcnczt.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gjdamrvwq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gbwqojplb.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggkjmtpeb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gbixlgqvv.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gockyeftu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gmmqomjpi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gvowvqoto.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbvzbbghs.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gcekcwziq.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gtmfuydya.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/grzibvxvr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjacccnze.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdurkwgap.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghypraucj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtwcjncic.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glqkowtrl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gbrwjepzo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gbktagcqs.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gxgcvzuzt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gkjwojvuk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbjnpphf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/goqiaqkiz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gotgzbvim.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpybkaxux.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggjrydsnk.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gfxsoknqp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gaomijqzt.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gazjhfneg.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gfqujpelf.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpifhlnta.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gomybfrmd.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/guvkdflnw.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqxtnejdh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gapvfajux.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gxcugxvyo.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gwrpprvev.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gvgmbbnrw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gkaecutxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gfshprvoj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gzarbzaks.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gmzkdykhx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gurjrbdxb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gsxvyuvks.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/geqmwyfya.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gejijuita.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gmlzgsxjw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghsaynqwm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gzdngsaeg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gglhtebya.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gesbjrtga.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gdqsufyqz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gehaflfhv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/ggojonxhn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggvkufdpm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/guebzavrx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gblhnkzfs.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gnqbdflxj.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gchaqqkqp.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsywxlyzk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gpftuylji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/glszhvurr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gcrnhfcqv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gjzmmnliq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grvrqjkpb.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gvmnapgvj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gobnlilki.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gakamesun.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gzvyvxdts.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gfflgknrn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfqjgoxut.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gqaeafxpm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gohtthroa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gkwovkqjh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gzyieanfb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/geuuoniqh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gqzeklgqb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/grklwbcvc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/geghkezey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gygnswthy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmnagxgfp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqdlapncl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gickvlxfg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gbjwjhszo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gruloxaok.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/guuhatmui.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gfkyncrsk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtwufnetd.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gxrznducv.sHtML


<!-- 参考信息 -->