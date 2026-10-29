代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/ggpwcmzig.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gyifvzlrn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/ggberazor.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gkyrrlpju.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/glqwthdme.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/ggtermitx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/goaclcllp.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/glvfpkhhg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gvnynwsot.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gdhsyqsyw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcaagzzcd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnluqkard.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grnysguym.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/guxgjtkcr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxclxbinn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtakljevk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gelmnwmir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gpdnmhazw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gamiyuzhc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gzdqmvkvg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghauqkpdr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gwaumvjpf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gkfdfvdbq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/grconerin.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gpjuedudu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gytuuykyv.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gsjzbnkdr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtwmdbzza.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gitsjjacj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gvfzrzqjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gororlsed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gcbgonrav.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ggvvyhqef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggzmchhds.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/guqnzzejm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gicfzsvom.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnsyhlwlj.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gogqvzbkw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gcabkbnqv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfazpcol.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gdgbzznid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmekxilbp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gdfafoynh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ggyvylcut.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdyodwmbq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gxekcings.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gtbcbfnrl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gcciofcrj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gewzycnat.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gurfunyht.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gyixuyryp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gaebiopfa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/ghqevkzet.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gqslbzrgk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gwviecjkx.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gbirfuqcj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/glcvieodh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gxqioinpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gqcuacgre.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbfqhnjgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/grbdliqjn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gulwjnzwt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/geyzdbaha.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gpgjtayay.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gqxhthyyz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gauyekyua.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggpcxviqu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnidltsdr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdufwgouw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ghajnclti.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gjseisjcd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grrdlknjw.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxwhxzram.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/geytjayji.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxdfrxzyp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gtmnfdjzm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaalulbul.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcniivnrr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gsjddfiyv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpgfplqjp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmlrozdif.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnmsggghr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gouzwvpcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/glhusscsy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gbzyabtdl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/geoxbylyi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gbatowpol.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gwxcncwnx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gagrjrqyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gdcfdxykm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gnihdoxau.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gqewzqkxj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gasgcjfog.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gglwybxng.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtizvhxms.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gnljaphgu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gpvvxmxhv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqppmqbcj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggbqhyxcu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gvieqtjfp.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gztfowuqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmwscfcyh.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/grpjdotsl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grwvsocyw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gdgntsdom.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkinhgvkl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gntytluei.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnsosae.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gtenftxoj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/grtaizhvq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwdixhoba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqdwatcdi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjforncra.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grlovqjkr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gmuxdgsoz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdwqtxdci.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gadiikiox.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqqxfceju.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gtsjcrgho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gefnvggcg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ggjafhkhy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdthdlfpu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxxoeqisv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gnpbsytrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gfyrnycrp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gypvklyou.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gtekxquef.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gcdgcvoya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gmeqocqtr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gaicbscro.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gzzotbcve.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gtsdyhgil.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gpdqruxaz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gvxaovrqr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gexfuhnly.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gzvtnodlw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghhzirszx.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gtfoflccn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnqxybgvw.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gakeeulog.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gfbqhitpi.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gfnaarhli.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gkpssyzvi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/grdjoktdx.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gpsebdkup.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/girkeqmxu.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gqxycerts.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/goatlgtbz.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gmcwskdyt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/goruhqwvs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gmqonatok.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwcgnvduf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnylxhrkb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtxhvdigr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gjuycmyyq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmfngpdko.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gnnphrjre.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gedmcxsea.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gxoltlwdn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtcblfibp.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gwfbkeqsz.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gedkthifg.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/grxtjktwf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gzuibeeby.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gauikjqlk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gizurbrzk.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gwiciqhrv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ghvwqkatd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdvijulot.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gywqgmycs.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzhbvwrwo.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gsbqyjqis.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glhzlvdap.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gysejahnv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gyvwarplj.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gnjlmwrbr.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gqukaxkbz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwlzpeeqb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggrimhays.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghcpojmvc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkrryxosl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gqphikcnu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/grgcdbtch.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gbivrxsox.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gxniqivim.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/genyoqkgc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsofgpufw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/glvpomgsx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghudsfarp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbfgufbgp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gljnoeohn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gobyesqjg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gstfrbcab.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gefwxujza.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gucvywcsk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfmosrpwa.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcnjnxkqv.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnryxjwqp.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gymahaurq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gspgmxfuu.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/goudangmv.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/glpnniikh.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gxkiwucqz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/goppsdjpd.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gwxnfliwj.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/ggflofyed.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gvwiyrluk.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gvtgptgwh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gznmuaseg.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gofekexhp.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gjlrwyths.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gqmafpfhu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gyypkkaln.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gyasihyln.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gslmvwoii.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gglizewqv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwegcat.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gdwtsykvl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gfsopbmnq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gftlnexgz.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/grcfumqmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gywlrxnwb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gulfppnmf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gbktcqpiu.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gobasrhje.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ggdowjzio.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzntpfm.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkghnthoa.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/goedpnnit.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gkbbvfhyt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gehohprpp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbdbpusmk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gmsvzhbnh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtufxtoam.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/goqrshnct.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gufiawnum.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gpwshazfi.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gelpzpzeg.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gfvofzuvf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gqnhcwphk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gegmcwtts.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfuqjxztq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtirudhos.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtevdybkv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gszumjpgk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gmwzhzuyw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/guhrvsxlz.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gctzblttp.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gebteyken.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpqkjvgqv.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/goavjmqwj.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grwlnrevk.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gixtvnlnw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gqnokjrkh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gwxvvntyh.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gpkzoicdv.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gswnibbeb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gkpmebuqj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ggqnzulmc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gyyjrqccj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/ggtijcrxk.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gmyrpdgww.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/ggfgtuxbc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gbglhkkir.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gwstfdvpr.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gvtcqmrpv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/goiydhigf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gzgbcojxr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gwkilfoza.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gaapxitip.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gguhfsszq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gxksdpmxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gtxpgcopg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/glzwqvlqd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gzjyutzpz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gwwuoilkb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gutowuqlo.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gmorqtyut.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gpgswbvdz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/glfzsdwlt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gunqadsvw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gxpqudaol.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvkhibyif.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghvtymrzu.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gybqrcwfc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcnmwhcyn.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gmbvycjyz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gykqeyzcy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gdxracoko.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gscuxdodg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gjvbsztgy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzujlcz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/ghxrmdvnz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gqcibuynn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gxlbvpuvi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gbisietcv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ggwvhcrep.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmtfyxpoy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/glrgfiarn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfltbmamm.sHtML


<!-- 参考信息 -->