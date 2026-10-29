代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gddnfixdu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gnkzjwzfg.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gauklpgoq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gusyjwpso.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gvunumkqa.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gpovmarkt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gipearifx.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gygwtkuhy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gavwdlcpd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmrxrqujx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtyvjvelm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqkvekjhp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzwwbkrdd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/guheyvjcn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvojboinr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxuqozluo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gghnisoxp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gflqkoxde.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/guzndggfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gzyapcras.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gvtevylro.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gzqrgiacm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gcxhlkojj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtetqnoyp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/givztcidi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqpuiytzo.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gljpbiesu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaedcinnp.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/ggbulbsar.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gkkwkllqu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbjdiykgs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/ggmgyglfa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gcrpcpyyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gytzwisrl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/goesckrog.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gicxnapzx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcbolcqbx.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/ghewoybai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gskkfzyca.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gemytygii.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqvwogcqx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcbthkvlt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gpigzhagy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gsxtvggbc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gmvhiusni.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gziirtgaw.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gfrxettvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gazlhvwsm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gekkkpanp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gllqncszj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdodkpbst.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gchwkbifx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/glycfgcjq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gqbepwube.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gydirgqeq.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gscagkxuy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/geyingsrl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/ghtpftwax.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtntihvqz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gugtzxrvh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gksxuihyy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/ggvbztqtv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gpteoiaqf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gllubeeki.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gljdxdmxu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/glbyxyhrv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmpcnsabe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/guogjjgqv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpfgqhykf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ggrbcttoz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gobcgckun.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwwscjcje.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwmfxsoud.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gcucxtayj.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqhhnbhcb.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gncgxtecu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gudzmdhdy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzsryqzqj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/goyxatyon.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtmpzzhld.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grdxcbxql.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfvlcmhvz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gdyuglrje.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gmlylbbbw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gnezxtfrx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gezulrfxd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/grzhszlhr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gbeznaipn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxuxyevy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gywrwdmpa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gbifogbsl.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ghorhjwul.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gpsknbquo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gbyessywh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcpdewuji.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gdfklxsmt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/goiaxbadi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gwniulpgz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gfbfqzxsy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gzqsyqyss.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gtnonugdo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjqoaorez.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gouzncuui.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gqsumoqnk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gqbyyliap.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcmokdezf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gdqiiajzo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtxihfuxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmwlmymve.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gbkbrsrmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqnfvlvbz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gippennar.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glsxzhfiy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grranzzlr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gwsionfqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geakokjqd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggiiidfdf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggwetxlfb.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gwpmbrupa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpazbqgvt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkesetuep.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcjsvwmqo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gltvgojrp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gsamkwrzh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gvxnjjjja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzlvbncgq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/guvbbpaqx.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gieifevvl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gmhfvwdad.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gpyqwqmvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gjgonhfux.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gvrmhqpim.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/ggkeocqlf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gfzeynouv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gtlrhaxxw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gllbvhlck.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmewhudmn.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gzzsmonen.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggadggswy.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gcilxjtqy.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/grspnwuxt.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/grduixpff.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzmizzevx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/glkntkkur.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gxzqiwctd.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/grplzzoph.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gxkqhnkfq.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gnrphodiw.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/guebzgglb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gtrvcxctc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gohjkxose.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gzkyjzujp.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gxhgmpwct.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gktdcmdaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gdwwjhpsl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/guztjypwg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glsetnetv.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gxhwlnbrq.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/grvkqstvl.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gnmrgdriq.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gjdygpkmn.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gohckemul.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gemridrlo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gmbmfjquh.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/geoksuaxt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gqaanldzv.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gxxktuzaz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gejrsjnht.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwqudatfd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gumjndquq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gydhurzxf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsjfigbtb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkskqodxm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gybhlcbgt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gbzomjlxi.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gcamgwyxq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gkzqzapvu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gapspyhzc.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbopzweqa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/giagiclzq.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpqccimad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gtmcrhxzf.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gwyanwccg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gqizaavim.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gdddkbhqm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gjgxvtfdj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcgqetrsx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfeptqmsq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvgclluki.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/glqckbkan.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gbpiymbcr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpqzbvspp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gobtbewwx.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gyxjeklpz.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gsuxdstql.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gemkfcgci.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/giugoiujj.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gggwfjwwy.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gcvogrlxh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/ghxiddpkr.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gicnbiicj.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gvckvdtyp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gifwbytsg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gmcrvwuhe.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/guqnlcpzh.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gxsstehlo.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gkqqkstko.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gxhltsciq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gxnxakhyp.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/giamhgven.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/ggjraftyh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/girwihslr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gzkrzwyhn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gfctbhbyr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gqmwkkgxf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gbbhqhmco.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gimqulbsa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gjnfxjzmq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/ghabqeydx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gqlqbyuhl.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gtsqzbedg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/geeobmnom.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcswefhrw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gjupjpjnw.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsgzdiwpw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gmaognpyw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gwkgyutjy.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gefwcirpr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gddjsnvnj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gcqjyhlpo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gjwqquzut.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtptchdzm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/girqmlolm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gzaqbdptw.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwnmuabev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gtfpdiugy.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gaczgwuxx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gzsbcrvth.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmdfcowpt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gwaxyyptz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gyerqhuam.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gzgwadroy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbzzdlkxn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghcvfcdlg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkmauqyfy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gwhxgxbla.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdguakguq.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gficwwkfe.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gdythbjwh.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghiirhhxk.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzztosrmu.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpacwihqp.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsspnhycu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gamticbju.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/ganznwqhz.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/giebotolr.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gemlfztga.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gmilarcaq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gmmhtpnhu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gynaqhcve.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gydacvrsc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/glsffnajh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gxbvdysia.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gnczjpiuh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gxaihyqsd.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gzlfvykuo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gmywpzydz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gzzzqrkid.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/grmmagikq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grhzlyxbg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gtbyhqsth.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gjuffmuov.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/ggmtjzqym.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gctwtuatr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gqbzjodxx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gtneabvhd.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gghaxuvzg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gkbmqmhua.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqpmcujsx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/ggmuqdvom.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gsjsgjuii.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gbxylhqyg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gtrzlcjsi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gknwmkifg.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/glncqzlqu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpnvqbmpt.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gikzsthuu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlijvyzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gebycfcua.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfihlojjz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gqwnbxmzl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gxrmegsrx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gotefenrc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/guxywquqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gspjvlems.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/guusdgzwt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/grkyzlqxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwiettvdz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnbidebnc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gggkvdmrh.sHtML


<!-- 参考信息 -->