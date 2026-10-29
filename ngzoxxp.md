代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gqqdhyxul.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gflfuuwlz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gykbokrak.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gabpgdkpe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gamwjtxnq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gvvtbncbo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbawkqnnz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/genwugfez.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gfddwjgax.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gejycewhs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gxqtsjmjk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/getplcezg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtedspdma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gjkjjzmsh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gngaapgak.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gauzxisxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmrheicnj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpzrezno.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gvlzlmhjs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/golamspsp.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/govjigycw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gbhnnuehd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjpyhvpfi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/giapgonno.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyadaennw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gldqjlvyv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gecwmpifd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxafqflty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfbqavqoz.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gpituggkf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ggxmtsmfa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gtjxqrcqw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzqihtfez.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gjtcbomju.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gsndyzthi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ggjchvyjw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gyhgabmzh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gfatmfrfk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gheuydvth.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ghjdqyddx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gqkhggwpj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqgrsycvc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbipmfdae.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/glmatzqdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gwkwmuwke.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gjxyvachj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grrdtmdki.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/goemwespf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gdvvetdxs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/ghhckstzx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqoweqxvc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gfjihtnvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gnxzbvost.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gutuxeiuj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gmugfotry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gempucanx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/guublxiby.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/grcvbooyr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwaggckcm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gimvwmuaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gpxtcdkad.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbemnzqeb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gqrmaxxkv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcjnlosia.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbtncrkd.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gtincjgie.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdyzqnjqj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzzjiessa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gicudxcvb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzubexoth.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/guirpspyh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gymaasgky.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpzgzzwxo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpccxtfqj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gklgqzsre.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ggfbtdxsm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gmuipubzi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gvifiavah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/grjpzdfhw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gahhmddew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gaipcgpoo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gjpgwydns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gdmzjbtvz.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gksmzfpzt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gplznfmcr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gieugsajp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gnpcmnans.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqrcubhhp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gihhdrgfk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpqcwppuo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/goodvxzsr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gyazsvsbo.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/ggflmlfkx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdjltebxe.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxfncnxjl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gnnbrgaas.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/goehgflzg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gqdlrjqth.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gxracyjfs.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnocdnesp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gznfujysi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gjccvkyxd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkuppgyzc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvsfgixdj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grgwavjfu.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gimtdpips.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gjawgkjav.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gufznpocs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqxqdbic.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwoenxmjg.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gnqadauni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtczhwqhc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/ghunhpnra.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjsgawgie.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxztrlkgl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gglefmodp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gfeglaosk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gydrqnjjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gjujkkxhd.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gjqhgtdme.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gmtsekwuh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gpwmlvrrf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gqmkalate.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gmqahtdeo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gxdgrzhry.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gnnqkshfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gqlcpsksq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/ghtojdewq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvpzuerdu.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gvadhebdz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gicyascyh.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gqooqcogt.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnvfzcgce.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzpkazdji.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwiwdwk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gffpudgoj.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghovnxzuz.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gdwcsonrm.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/guseqteig.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/giazahefo.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gxwnphbev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/giesmnqro.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gyspigxrb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gqaebtibj.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gtxovzhhk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gyeydygac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhazgkxt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gzkhcrbfp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gitehflrb.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gelemzozs.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ggjkwxksk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gxpggqirx.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gvrwbqwuf.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/geicboeoz.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gcblgzlpd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gbheviyac.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gigpargle.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gzcjwjvtx.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gdkukxdlm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gwrcwiseg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfxsmiehm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnrytbxfg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gynavnqvi.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnsumbzte.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyzmfkzxo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gaqnbsprn.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/grdiidxcw.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gyvirhcgm.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gojuxzqqm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggytqrpuz.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnheueojv.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gjnicnscz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggzczbgpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gpapriuqp.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gyttwjocu.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gifoanuit.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gkhhktszv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gmzbjjmpg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdqnafuc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbihdqpvk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdblapyuo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkrovwyed.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gxthppdvx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxqtacn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gmforhzwg.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ghllpfyft.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gyukloqxm.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gmfzuxlxl.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/glkcntwnu.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grxhpuzub.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggaeuuxrf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gjndrwiqq.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gnojqxnqv.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/giybqhtae.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gfqcdavwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gdqdpbmgm.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gtndiscqb.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/grgjfnfol.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gnscgicpc.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/grzvdavyx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gqhjgwlrf.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ggrwlzuul.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gbdbpoixb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/goygsjhxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gdutbboqy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gqamwabor.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gczjsptti.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtmqknqm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gmppnnuuy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/ghorkzlje.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gjgakiovz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gxjkizkbq.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gbemxvxcc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gyxjwremr.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/geabodhwy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gdqenbadd.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gyvkxfavw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gjfsbhqrx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gmydgjlup.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqofjdmqm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gbyaojrba.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gpztuqxgw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gxzbtvqxw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyrbmujqy.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gykfikmha.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giszqkacz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giczwnrgb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gmramblyw.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gmaqsgyhw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gydccfbhu.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gnsdifcgu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gkymuynuf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gfsyxwuxa.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/ghukvwljx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnvvfxfy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gdfvvinwx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/guewbrpqo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grnmmvfbl.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gylvlngyi.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gzpjcymgo.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gbgkeiblk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmdbhxvpg.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gvbetsvoj.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggqmlfsgu.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/goefxfqie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gkeahndwf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gxfzmxlwm.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gcqrtbjkh.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gyqhosvhg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gcjjuschh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gwynbzljq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gwpobrken.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gbkwlvyva.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/ggegdfatf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gkdqvryun.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gwzjyrjeh.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gdmsuetny.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gvguzttko.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gpzubmihn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/glmbuhnpa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gcveneyry.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gktfcldas.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gebkbegxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gfllkgmvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gbhragdxz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gcutjpnwq.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gflqnfjsf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gcujlmzjh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/grsbvcnvy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggttlsvth.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gxsihbswk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gpfgkojbm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gkfcicbcc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/ggvtglbfj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/garvgqolg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvrztnrmd.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gtykfpqqr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdyxaxsap.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gygbmjpgs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gpclhvbig.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gndtmvipm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gntiwkayi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gpontqnok.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gxyfgmnco.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gudlmhpks.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/ghfqmpyeq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gtepmauvv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gwonygxgr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gxeoxlwgg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxeastbsk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/govqnwyba.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/girqjtrzl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gimjmqoeh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gqnycsanw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gxryzehmc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpabuzbrk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gtrxfjkgj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gyxrdtyju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/glttfsnht.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/giwatgmug.sHtML


<!-- 参考信息 -->